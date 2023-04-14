# Comparing `tmp/syft-0.8.0b6.tar.gz` & `tmp/syft-0.8.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.0b6.tar", last modified: Sun Apr  9 12:33:59 2023, max compression
+gzip compressed data, was "syft-0.8.0b7.tar", last modified: Fri Apr 14 05:00:31 2023, max compression
```

## Comparing `syft-0.8.0b6.tar` & `syft-0.8.0b7.tar`

### file list

```diff
@@ -1,133 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.383129 syft-0.8.0b6/
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-09 12:31:26.000000 syft-0.8.0b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 12:31:26.000000 syft-0.8.0b6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-04-09 12:33:59.383129 syft-0.8.0b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-04-09 12:31:24.000000 syft-0.8.0b6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-09 12:31:26.000000 syft-0.8.0b6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-09 12:33:59.387129 syft-0.8.0b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-09 12:31:26.000000 syft-0.8.0b6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.359127 syft-0.8.0b6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.363127 syft-0.8.0b6/src/syft/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-09 12:31:42.000000 syft-0.8.0b6/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-09 12:31:42.000000 syft-0.8.0b6/src/syft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.367128 syft-0.8.0b6/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.367128 syft-0.8.0b6/src/syft/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.367128 syft-0.8.0b6/src/syft/core/node/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.383129 syft-0.8.0b6/src/syft/core/node/new/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    26475 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/action_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/action_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/action_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/action_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/capnp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/data_subject_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/dataset_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/message_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/message_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/metadata_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    14193 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/network_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/node_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/project_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/project_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    16030 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/sqlite_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/third_party.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/worker_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    23988 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/experimental_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.383129 syft-0.8.0b6/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.383129 syft-0.8.0b6/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15416 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/gevent_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/user_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.367128 syft-0.8.0b6/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-04-09 12:33:59.000000 syft-0.8.0b6/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-09 12:33:59.000000 syft-0.8.0b6/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:33:59.000000 syft-0.8.0b6/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:33:59.000000 syft-0.8.0b6/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-09 12:33:59.000000 syft-0.8.0b6/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 12:33:59.000000 syft-0.8.0b6/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.472833 syft-0.8.0b7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-14 04:57:50.000000 syft-0.8.0b7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 04:57:50.000000 syft-0.8.0b7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-04-14 05:00:31.472833 syft-0.8.0b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-04-14 04:57:50.000000 syft-0.8.0b7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-14 04:57:50.000000 syft-0.8.0b7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-14 05:00:31.476833 syft-0.8.0b7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-14 04:57:50.000000 syft-0.8.0b7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.436833 syft-0.8.0b7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.444834 syft-0.8.0b7/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-14 04:58:05.000000 syft-0.8.0b7/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-04-14 04:58:05.000000 syft-0.8.0b7/src/syft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.448834 syft-0.8.0b7/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.448834 syft-0.8.0b7/src/syft/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.448834 syft-0.8.0b7/src/syft/core/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.468834 syft-0.8.0b7/src/syft/core/node/new/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26657 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/data_subject_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/dataset_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19254 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/message_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/message_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/metadata_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14193 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/node_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21086 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/project_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12210 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/sqlite_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16320 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/third_party.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_policy_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/worker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/experimental_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.468834 syft-0.8.0b7/src/syft/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.472833 syft-0.8.0b7/src/syft/external/oblv/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15416 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/gevent_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/user_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.444834 syft-0.8.0b7/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-04-14 05:00:31.000000 syft-0.8.0b7/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-14 05:00:31.000000 syft-0.8.0b7/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 05:00:31.000000 syft-0.8.0b7/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 05:00:31.000000 syft-0.8.0b7/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-14 05:00:31.000000 syft-0.8.0b7/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 05:00:31.000000 syft-0.8.0b7/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.0b6/LICENSE` & `syft-0.8.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/PKG-INFO` & `syft-0.8.0b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.0b6
+Version: 0.8.0b7
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.0b6 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.0b7 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.8 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.0b6/README.md` & `syft-0.8.0b7/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/setup.cfg` & `syft-0.8.0b7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.0-beta.6"
+version = attr: "0.8.0-beta.7"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -82,14 +82,15 @@
 	pytest-parallel
 	pytest-asyncio
 	pytest-randomly
 	pytest-sugar
 	pytest_mock_resources
 	python_on_whales
 	pytest-lazy-fixture
+	pytest-rerunfailures
 	coverage
 	joblib
 	faker
 oblv = 
 	pyoblv==0.2.0
 
 [test]
@@ -101,14 +102,17 @@
 norecursedirs = 
 	dist
 	build
 	.tox
 testpaths = tests
 filterwarnings = 
 	ignore:.*Deprecated.*:DeprecationWarning
+markers = 
+	slow: marks tests as slow (deselect with '-m "not slow"')
+	flaky: mark tests that might fail from network unpredictable errors
 
 [aliases]
 dists = bdist_wheel
 
 [bdist_wheel]
 universal = 1
```

### Comparing `syft-0.8.0b6/src/syft/VERSION` & `syft-0.8.0b7/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.0-beta.6"
+__version__ = "0.8.0-beta.7"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.0b6/src/syft/__init__.py` & `syft-0.8.0b7/src/syft/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     IMPORTANT: syft.core should be very careful when importing functionality from outside of syft
     core!!! Since we plan to drop syft core down to a language (such as C++ or Rust)
     this can create future complications with lower level languages calling
     higher level ones.
 To begin your education in Syft, continue to the :py:mod:`syft.core.node.vm.vm` module...
 """
 
-__version__ = "0.8.0-beta.6"
+__version__ = "0.8.0-beta.7"
 
 # stdlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
 
@@ -45,24 +45,29 @@
 from .core.node.new.client import login  # noqa: F401
 from .core.node.new.credentials import SyftSigningKey  # noqa: F401
 from .core.node.new.data_subject import DataSubjectCreate as DataSubject  # noqa: F401
 from .core.node.new.dataset import CreateAsset as Asset  # noqa: F401
 from .core.node.new.dataset import CreateDataset as Dataset  # noqa: F401
 from .core.node.new.deserialize import _deserialize as deserialize  # noqa: F401
 from .core.node.new.messages import MessageStatus  # noqa: F401
+from .core.node.new.policy import CustomInputPolicy  # noqa: F401
+from .core.node.new.policy import CustomOutputPolicy  # noqa: F401
+from .core.node.new.policy import ExactMatch  # noqa: F401
+from .core.node.new.policy import SingleExecutionExactOutput  # noqa: F401
+from .core.node.new.policy import UserInputPolicy  # noqa: F401
+from .core.node.new.policy import UserOutputPolicy  # noqa: F401
 from .core.node.new.project import ProjectSubmit as Project  # noqa: F401
 from .core.node.new.request import SubmitRequest as Request  # noqa: F401
 from .core.node.new.response import SyftError  # noqa: F401
 from .core.node.new.response import SyftNotReady  # noqa: F401
 from .core.node.new.response import SyftSuccess  # noqa: F401
 from .core.node.new.roles import Roles as roles  # noqa: F401
+from .core.node.new.serializable import serializable  # noqa: F401
 from .core.node.new.serialize import _serialize as serialize  # noqa: F401
 from .core.node.new.uid import UID  # noqa: F401
-from .core.node.new.user_code import ExactMatch  # noqa: F401
-from .core.node.new.user_code import SingleExecutionExactOutput  # noqa: F401
 from .core.node.new.user_code import UserCodeStatus  # noqa: F401
 from .core.node.new.user_code import syft_function  # noqa: F401
 from .core.node.new.user_service import UserService  # noqa: F401
 from .core.node.worker import Worker  # noqa: F401
 from .deploy import Orchestra  # noqa: F401
 from .external import OBLV  # noqa: F401
 from .external import enable_external_lib  # noqa: F401
```

### Comparing `syft-0.8.0b6/src/syft/core/node/__init__.py` & `syft-0.8.0b7/src/syft/core/node/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/action_object.py` & `syft-0.8.0b7/src/syft/core/node/new/action_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,19 +150,19 @@
 
 def make_action_side_effect(context: PreHookContext, *args: Any, **kwargs: Any) -> Any:
     try:
         action = context.obj.syft_make_method_action(
             op=context.op_name, args=args, kwargs=kwargs
         )
         context.action = action
-    except Exception as e:
-        print(
-            "Exception detected in make_action_side_effect", e
-        )  # TODO: Put this Exception back
-        # pass
+    except Exception:  # nosec
+        # print(
+        #     "Exception detected in make_action_side_effect", e
+        # )  # TODO: Put this Exception back
+        pass
     return context, args, kwargs
 
 
 def send_action_side_effect(context: PreHookContext, *args: Any, **kwargs: Any) -> Any:
     try:
         if context.op_name not in dont_make_side_effects and hasattr(
             context.obj, "syft_node_uid"
@@ -172,30 +172,31 @@
                     action = context.obj.syft_make_method_action(
                         op=context.op_name, args=args, kwargs=kwargs
                     )
                     context.action = action
 
                 action_result = context.obj.syft_execute_action(action, sync=True)
                 if not isinstance(action_result, ActionObject):
-                    print("Got back unexpected response", action_result)
+                    # print("Got back unexpected response", action_result)
+                    pass
                 else:
                     context.node_uid = action_result.syft_node_uid
                     context.result_id = action.result_id
-                    print("IGNORING: got action result", action_result)
+                    # print("IGNORING: got action result", action_result)
             else:
                 # 🟡 TODO
                 pass
                 # print(
                 #     "Can't Send Action without a target node. Use .point_to(node_uid: UID)"
                 # )
-    except Exception as e:
-        print(
-            "Exception in send_action_side_effect", e
-        )  # TODO: Put this Exception back
-        # pass
+    except Exception:  # nosec
+        # print(
+        #     "Exception in send_action_side_effect", e
+        # )  # TODO: Put this Exception back
+        pass
     return context, args, kwargs
 
 
 def propagate_node_uid(context: PreHookContext, op: str, result: Any) -> Any:
     try:
         if context.op_name not in dont_make_side_effects and hasattr(
             context.obj, "syft_node_uid"
@@ -205,21 +206,23 @@
                 if not hasattr(result, "syft_node_uid"):
                     # print("result doesnt have a syft_node_uid attr")
                     pass
                 if op not in context.obj._syft_dont_wrap_attrs():
                     if hasattr(result, "syft_node_uid"):
                         setattr(result, "syft_node_uid", syft_node_uid)
                 else:
-                    print("dont propogate node_uid because output isnt wrapped")
+                    # print("dont propogate node_uid because output isnt wrapped")
+                    pass
             else:
                 # 🟡 TODO
                 # print("Can't proagate node_uid because parent doesnt have one")
                 pass
-    except Exception as e:
-        print("Exception in propagate_node_uid", e)
+    except Exception:  # nosec
+        # print("Exception in propagate_node_uid", e)
+        pass
     return result
 
 
 def is_action_data_empty(obj: Any) -> bool:
     if hasattr(obj, "syft_action_data"):
         obj = obj.syft_action_data
     if isinstance(obj, ActionDataEmpty):
@@ -326,14 +329,16 @@
 
     @staticmethod
     def from_obj(
         syft_action_data: Any,
         id: Optional[UID] = None,
         syft_lineage_id: Optional[LineageID] = None,
     ) -> ActionObject:
+        if isinstance(syft_action_data, ActionObject):
+            return syft_action_data
         if id and syft_lineage_id and id != syft_lineage_id.id:
             raise Exception("UID and LineageID should match")
         action_type = action_type_for_type(syft_action_data)
         if action_type is None:
             raise Exception(f"{type(syft_action_data)} not in action_types")
         action_object = action_type(syft_action_data=syft_action_data)
         if id:
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/action_service.py` & `syft-0.8.0b7/src/syft/core/node/new/action_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,74 +136,77 @@
         )
         if result.is_ok():
             return Ok(result.ok())
         return Err(result.err())
 
     # not a public service endpoint
     def _user_code_execute(
-        self, context: AuthedServiceContext, code_item: UserCode, kwargs: Dict[str, Any]
+        self,
+        context: AuthedServiceContext,
+        code_item: UserCode,
+        kwargs: Dict[str, Any],
     ) -> Result[ActionObjectPointer, Err]:
         filtered_kwargs = code_item.input_policy.filter_kwargs(
             kwargs=kwargs, context=context, code_item_id=code_item.id
         )
+
         if filtered_kwargs.is_err():
             return filtered_kwargs
         filtered_kwargs = filtered_kwargs.ok()
         has_twin_inputs = False
-        kwargs = {}
+
+        real_kwargs = {}
         for key, kwarg_value in filtered_kwargs.items():
             if isinstance(kwarg_value, TwinObject):
                 has_twin_inputs = True
-            kwargs[key] = kwarg_value
+            real_kwargs[key] = kwarg_value
 
         result_id = UID()
 
         try:
             if not has_twin_inputs:
                 # no twins
-                filtered_kwargs = filter_twin_kwargs(kwargs, twin_mode=TwinMode.NONE)
+                filtered_kwargs = filter_twin_kwargs(
+                    real_kwargs, twin_mode=TwinMode.NONE
+                )
                 exec_result = execute_byte_code(code_item, filtered_kwargs)
                 result_action_object = wrap_result(
                     code_item.id, result_id, exec_result.result
                 )
             else:
                 # twins
-                private_kwargs = filter_twin_kwargs(kwargs, twin_mode=TwinMode.PRIVATE)
+                private_kwargs = filter_twin_kwargs(
+                    real_kwargs, twin_mode=TwinMode.PRIVATE
+                )
                 private_exec_result = execute_byte_code(code_item, private_kwargs)
                 result_action_object_private = wrap_result(
                     code_item.id, result_id, private_exec_result.result
                 )
 
-                mock_kwargs = filter_twin_kwargs(kwargs, twin_mode=TwinMode.MOCK)
+                mock_kwargs = filter_twin_kwargs(real_kwargs, twin_mode=TwinMode.MOCK)
                 mock_exec_result = execute_byte_code(code_item, mock_kwargs)
                 result_action_object_mock = wrap_result(
                     code_item.id, result_id, mock_exec_result.result
                 )
 
                 result_action_object = TwinObject(
                     id=result_id,
                     private_obj=result_action_object_private,
                     mock_obj=result_action_object_mock,
                 )
         except Exception as e:
-            print("what is this exception", e)
-            return Err("_user_code_execute failed")
+            return Err(f"_user_code_execute failed. {e}")
 
         set_result = self.store.set(
             uid=result_id,
             credentials=context.credentials,
             syft_object=result_action_object,
         )
         if set_result.is_err():
             return set_result.err()
-
-        if isinstance(result_action_object, TwinObject):
-            result_action_object = result_action_object.mock
-        result_action_object.syft_point_to(context.node.id)
-
         return Ok(result_action_object)
 
     @service_method(path="action.execute", name="execute", roles=GUEST_ROLE_LEVEL)
     def execute(
         self, context: AuthedServiceContext, action: Action
     ) -> Result[ActionObjectPointer, Err]:
         """Execute an operation on objects in the action store"""
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/action_store.py` & `syft-0.8.0b7/src/syft/core/node/new/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/action_types.py` & `syft-0.8.0b7/src/syft/core/node/new/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/api.py` & `syft-0.8.0b7/src/syft/core/node/new/api.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/array.py` & `syft-0.8.0b7/src/syft/core/node/new/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/arrow.py` & `syft-0.8.0b7/src/syft/core/node/new/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/client.py` & `syft-0.8.0b7/src/syft/core/node/new/client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/connection.py` & `syft-0.8.0b7/src/syft/core/node/new/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/context.py` & `syft-0.8.0b7/src/syft/core/node/new/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/credentials.py` & `syft-0.8.0b7/src/syft/core/node/new/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/data_subject.py` & `syft-0.8.0b7/src/syft/core/node/new/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/data_subject_member.py` & `syft-0.8.0b7/src/syft/core/node/new/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/data_subject_member_service.py` & `syft-0.8.0b7/src/syft/core/node/new/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/data_subject_service.py` & `syft-0.8.0b7/src/syft/core/node/new/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/dataset.py` & `syft-0.8.0b7/src/syft/core/node/new/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/dataset_service.py` & `syft-0.8.0b7/src/syft/core/node/new/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/dataset_stash.py` & `syft-0.8.0b7/src/syft/core/node/new/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/datetime.py` & `syft-0.8.0b7/src/syft/core/node/new/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/decorators.py` & `syft-0.8.0b7/src/syft/core/node/new/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/deserialize.py` & `syft-0.8.0b7/src/syft/core/node/new/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/document_store.py` & `syft-0.8.0b7/src/syft/core/node/new/document_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # stdlib
 from functools import partial
 import sys
 import types
 import typing
 from typing import Any
+from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import Union
 
@@ -20,14 +21,17 @@
 from result import Ok
 from result import Result
 from typeguard import check_type
 
 # relative
 from ....telemetry import instrument
 from .base import SyftBaseModel
+from .locks import LockingConfig
+from .locks import NoLockingConfig
+from .locks import SyftLock
 from .response import SyftSuccess
 from .serializable import serializable
 from .syft_object import SYFT_OBJECT_VERSION_1
 from .syft_object import SyftBaseObject
 from .syft_object import SyftObject
 from .uid import UID
 
@@ -312,14 +316,17 @@
         settings: PartitionSettings,
         store_config: StoreConfig,
     ) -> None:
         self.settings = settings
         self.store_config = store_config
         self.init_store()
 
+        store_config.locking_config.lock_name = settings.name
+        self.lock = SyftLock(store_config.locking_config)
+
     def init_store(self) -> Result[Ok, Err]:
         try:
             self.unique_cks = self.settings.unique_keys.all
             self.searchable_cks = self.settings.searchable_keys.all
         except BaseException as e:
             return Err(str(e))
 
@@ -333,37 +340,87 @@
 
     def store_query_key(self, obj: Any) -> QueryKey:
         return self.settings.store_key.with_obj(obj)
 
     def store_query_keys(self, objs: Any) -> QueryKeys:
         return QueryKeys(qks=[self.store_query_key(obj) for obj in objs])
 
-    def find_index_or_search_keys(self, index_qks: QueryKeys, search_qks: QueryKeys):
-        raise NotImplementedError
+    # Thread-safe methods
+    def _thread_safe_cbk(self, cbk: Callable, *args, **kwargs):
+        locked = self.lock.acquire(blocking=True)
+        if not locked:
+            return Err("Failed to acquire lock for the operation")
 
-    def all(self) -> Result[List[BaseStash.object_type], str]:
-        raise NotImplementedError
+        try:
+            result = cbk(*args, **kwargs)
+        except BaseException as e:
+            result = Err(str(e))
+        self.lock.release()
+
+        return result
 
     def set(
+        self, obj: SyftObject, ignore_duplicates: bool = False
+    ) -> Result[SyftObject, str]:
+        return self._thread_safe_cbk(
+            self._set, obj=obj, ignore_duplicates=ignore_duplicates
+        )
+
+    def find_index_or_search_keys(
+        self, index_qks: QueryKeys, search_qks: QueryKeys
+    ) -> Result[List[SyftObject], str]:
+        return self._thread_safe_cbk(
+            self._find_index_or_search_keys, index_qks=index_qks, search_qks=search_qks
+        )
+
+    def remove_keys(
+        self,
+        unique_query_keys: QueryKeys,
+        searchable_query_keys: QueryKeys,
+    ) -> None:
+        self._thread_safe_cbk(
+            self._remove_keys,
+            unique_query_keys=unique_query_keys,
+            searchable_query_keys=searchable_query_keys,
+        )
+
+    def update(self, qk: QueryKey, obj: SyftObject) -> Result[SyftObject, str]:
+        return self._thread_safe_cbk(self._update, qk=qk, obj=obj)
+
+    def get_all_from_store(self, qks: QueryKeys) -> Result[List[SyftObject], str]:
+        return self._thread_safe_cbk(self._get_all_from_store, qks)
+
+    def delete(self, qk: QueryKey) -> Result[SyftSuccess, Err]:
+        return self._thread_safe_cbk(self._delete, qk)
+
+    def all(self) -> Result[List[BaseStash.object_type], str]:
+        return self._thread_safe_cbk(self._all)
+
+    # Potentially thread-unsafe methods.
+    # CAUTION:
+    #       * Don't use self.lock here.
+    #       * Do not call the public thread-safe methods here(with locking).
+    # These methods are called from the public thread-safe API, and will hang the process.
+    def _set(
         self,
         obj: SyftObject,
         ignore_duplicates: bool = False,
     ) -> Result[SyftObject, str]:
         raise NotImplementedError
 
-    def update(self, qk: QueryKey, obj: SyftObject) -> Result[SyftObject, str]:
+    def _update(self, qk: QueryKey, obj: SyftObject) -> Result[SyftObject, str]:
         raise NotImplementedError
 
-    def get_all_from_store(self, qks: QueryKeys) -> Result[List[SyftObject], str]:
+    def _get_all_from_store(self, qks: QueryKeys) -> Result[List[SyftObject], str]:
         raise NotImplementedError
 
-    def create(self, obj: SyftObject) -> Result[SyftObject, str]:
+    def _delete(self, qk: QueryKey) -> Result[SyftSuccess, Err]:
         raise NotImplementedError
 
-    def delete(self, qk: QueryKey) -> Result[SyftSuccess, Err]:
+    def _all(self) -> Result[List[BaseStash.object_type], str]:
         raise NotImplementedError
 
 
 @instrument
 @serializable()
 class DocumentStore:
     """Base Document Store
@@ -472,15 +529,15 @@
         self, **kwargs: Dict[str, Any]
     ) -> Result[Optional[BaseStash.object_type], str]:
         return self.query_one_kwargs(**kwargs)
 
     def find_and_delete(self, **kwargs: Dict[str, Any]) -> Result[SyftSuccess, Err]:
         obj = self.query_one_kwargs(**kwargs)
         if obj.is_err():
-            return obj.err()
+            return obj
         else:
             obj = obj.ok()
 
         if not obj:
             return Err(f"Object does not exists with kwargs: {kwargs}")
         qk = self.partition.store_query_key(obj)
         return self.delete(qk=qk)
@@ -524,14 +581,22 @@
     """Base Store configuration
 
     Parameters:
         store_type: Type
             Document Store type
         client_config: Optional[StoreClientConfig]
             Backend-specific config
+        locking_config: LockingConfig
+            The config used for store locking. Available options:
+                * NoLockingConfig: no locking, ideal for single-thread stores.
+                * ThreadingLockingConfig: threading-based locking, ideal for same-process in-memory stores.
+                * FileLockingConfig: file based locking, ideal for same-device different-processes/threads stores.
+                * RedisLockingConfig: Redis-based locking, ideal for multi-device stores.
+            Defaults to NoLockingConfig.
     """
 
     __canonical_name__ = "StoreConfig"
     __version__ = SYFT_OBJECT_VERSION_1
 
     store_type: Type[DocumentStore]
     client_config: Optional[StoreClientConfig]
+    locking_config: LockingConfig = NoLockingConfig()
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/grid_url.py` & `syft-0.8.0b7/src/syft/core/node/new/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/kv_document_store.py` & `syft-0.8.0b7/src/syft/core/node/new/kv_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,45 +114,65 @@
                 if pk_key not in self.searchable_keys:
                     self.searchable_keys[pk_key] = defaultdict(list)
         except BaseException as e:
             return Err(str(e))
 
         return Ok()
 
-    def set(
+    def __len__(self) -> int:
+        return len(self.data)
+
+    # Potentially thread-unsafe methods.
+    # CAUTION:
+    #       * Don't use self.lock here.
+    #       * Do not call the public thread-safe methods here(with locking).
+    # These methods are called from the public thread-safe API, and will hang the process.
+
+    def _set(
         self, obj: SyftObject, ignore_duplicates: bool = False
     ) -> Result[SyftObject, str]:
         try:
             store_query_key = self.settings.store_key.with_obj(obj)
-            exists = store_query_key.value in self.data
             unique_query_keys = self.settings.unique_keys.with_obj(obj)
             searchable_query_keys = self.settings.searchable_keys.with_obj(obj)
             ck_check = self._validate_partition_keys(
                 store_query_key=store_query_key, unique_query_keys=unique_query_keys
             )
+            exists = store_query_key.value in self.data
             if not exists and ck_check == UniqueKeyCheck.EMPTY:
                 self._set_data_and_keys(
                     store_query_key=store_query_key,
                     unique_query_keys=unique_query_keys,
                     searchable_query_keys=searchable_query_keys,
                     obj=obj,
                 )
             elif not ignore_duplicates:
                 return Err(f"Duplication Key Error: {obj}")
         except Exception as e:
             return Err(f"Failed to write obj {obj}. {e}")
         return Ok(obj)
 
-    def all(self) -> Result[List[BaseStash.object_type], str]:
-        return Ok(list(self.data.values()))
+    def _remove_keys(
+        self,
+        unique_query_keys: QueryKeys,
+        searchable_query_keys: QueryKeys,
+    ) -> None:
+        uqks = unique_query_keys.all
+        for qk in uqks:
+            pk_key, pk_value = qk.key, qk.value
+            ck_col = self.unique_keys[pk_key]
+            ck_col.pop(pk_value, None)
 
-    def __len__(self) -> Result[List[BaseStash.object_type], str]:
-        return len(self.data)
+        sqks = searchable_query_keys.all
+        for qk in sqks:
+            pk_key, pk_value = qk.key, qk.value
+            ck_col = self.searchable_keys[pk_key]
+            ck_col.pop(pk_value, None)
 
-    def find_index_or_search_keys(
+    def _find_index_or_search_keys(
         self, index_qks: QueryKeys, search_qks: QueryKeys
     ) -> Result[List[SyftObject], str]:
         ids: Optional[Set] = None
         errors = []
         if len(index_qks.all) > 0:
             index_results = self._get_keys_index(qks=index_qks)
             if index_results.is_ok():
@@ -176,48 +196,29 @@
         if len(errors) > 0:
             return Err(" ".join(errors))
 
         if ids is None:
             return Ok([])
 
         qks = self.store_query_keys(ids)
-        return self.get_all_from_store(qks=qks)
+        return self._get_all_from_store(qks=qks)
 
-    def remove_keys(
-        self,
-        unique_query_keys: QueryKeys,
-        searchable_query_keys: QueryKeys,
-    ) -> None:
-        uqks = unique_query_keys.all
-        for qk in uqks:
-            pk_key, pk_value = qk.key, qk.value
-            ck_col = self.unique_keys[pk_key]
-            ck_col.pop(pk_value, None)
-
-        sqks = searchable_query_keys.all
-        for qk in sqks:
-            pk_key, pk_value = qk.key, qk.value
-            ck_col = self.searchable_keys[pk_key]
-            ck_col.pop(pk_value, None)
-
-    def update(self, qk: QueryKey, obj: SyftObject) -> Result[SyftObject, str]:
+    def _update(self, qk: QueryKey, obj: SyftObject) -> Result[SyftObject, str]:
         try:
             if qk.value not in self.data:
                 return Err(f"No object exists for query key: {qk}")
 
             _original_obj = self.data[qk.value]
             _original_unique_keys = self.settings.unique_keys.with_obj(_original_obj)
             _original_searchable_keys = self.settings.searchable_keys.with_obj(
                 _original_obj
             )
 
-            # 🟡 TODO 28: Add locking in this transaction
-
             # remove old keys
-            self.remove_keys(
+            self._remove_keys(
                 unique_query_keys=_original_unique_keys,
                 searchable_query_keys=_original_searchable_keys,
             )
 
             # update the object with new data
             for key, value in obj.to_dict(exclude_none=True).items():
                 if key == "id":
@@ -235,25 +236,22 @@
                 obj=_original_obj,
             )
 
             return Ok(_original_obj)
         except Exception as e:
             return Err(f"Failed to update obj {obj} with error: {e}")
 
-    def get_all_from_store(self, qks: QueryKeys) -> Result[List[SyftObject], str]:
+    def _get_all_from_store(self, qks: QueryKeys) -> Result[List[SyftObject], str]:
         matches = []
         for qk in qks.all:
             if qk.value in self.data:
                 matches.append(self.data[qk.value])
         return Ok(matches)
 
-    def create(self, obj: SyftObject) -> Result[SyftObject, str]:
-        pass
-
-    def delete(self, qk: QueryKey) -> Result[SyftSuccess, Err]:
+    def _delete(self, qk: QueryKey) -> Result[SyftSuccess, Err]:
         try:
             _obj = self.data.pop(qk.value)
             self._delete_unique_keys_for(_obj)
             self._delete_search_keys_for(_obj)
             return Ok(SyftSuccess(message="Deleted"))
         except Exception as e:
             return Err(f"Failed to delete with query key {qk} with error: {e}")
@@ -366,15 +364,14 @@
     def _set_data_and_keys(
         self,
         store_query_key: QueryKey,
         unique_query_keys: QueryKeys,
         searchable_query_keys: QueryKeys,
         obj: SyftObject,
     ) -> None:
-        # we should lock
         uqks = unique_query_keys.all
 
         for qk in uqks:
             pk_key, pk_value = qk.key, qk.value
             ck_col = self.unique_keys[pk_key]
             ck_col[pk_value] = store_query_key.value
             self.unique_keys[pk_key] = ck_col
@@ -391,7 +388,10 @@
                 # coerce the list of objects to strings for a single key
                 pk_value = " ".join([str(obj) for obj in pk_value])
 
             ck_col[pk_value].append(store_query_key.value)
             self.searchable_keys[pk_key] = ck_col
 
         self.data[store_query_key.value] = obj
+
+    def _all(self) -> Result[List[BaseStash.object_type], str]:
+        return Ok(list(self.data.values()))
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/linked_obj.py` & `syft-0.8.0b7/src/syft/core/node/new/linked_obj.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,17 +55,22 @@
         cls,
         obj: SyftObject,
         service_type: Optional[Type[Any]] = None,
         node_uid: Optional[UID] = None,
     ) -> Self:
         if service_type is None:
             # relative
+            from .action_object import ActionObject
+            from .action_service import ActionService
             from .service import TYPE_TO_SERVICE
 
-            service_type = TYPE_TO_SERVICE[type(obj)]
+            if isinstance(obj, ActionObject):
+                service_type = ActionService
+            else:
+                service_type = TYPE_TO_SERVICE[type(obj)]
 
         object_uid = getattr(obj, "id", None)
         if object_uid is None:
             raise Exception(f"{cls} Requires an object UID")
 
         if node_uid is None:
             node_uid = getattr(obj, "node_uid", None)
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/message_service.py` & `syft-0.8.0b7/src/syft/core/node/new/message_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/message_stash.py` & `syft-0.8.0b7/src/syft/core/node/new/message_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/messages.py` & `syft-0.8.0b7/src/syft/core/node/new/messages.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/metadata_service.py` & `syft-0.8.0b7/src/syft/core/node/new/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/metadata_stash.py` & `syft-0.8.0b7/src/syft/core/node/new/metadata_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/mongo_client.py` & `syft-0.8.0b7/src/syft/core/node/new/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/mongo_codecs.py` & `syft-0.8.0b7/src/syft/core/node/new/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/mongo_document_store.py` & `syft-0.8.0b7/src/syft/core/node/new/mongo_document_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 # relative
 from .document_store import DocumentStore
 from .document_store import QueryKey
 from .document_store import QueryKeys
 from .document_store import StoreConfig
 from .document_store import StorePartition
+from .locks import LockingConfig
+from .locks import NoLockingConfig
 from .mongo_client import MongoClient
 from .mongo_client import MongoStoreClientConfig
 from .response import SyftSuccess
 from .serializable import serializable
 from .syft_object import StorableObjectType
 from .syft_object import SyftObject
 from .syft_object import SyftObjectRegistry
@@ -114,14 +116,20 @@
         if collection_status.is_err():
             return collection_status
 
         self._collection = collection_status.ok()
 
         return self._create_update_index()
 
+    # Potentially thread-unsafe methods.
+    # CAUTION:
+    #       * Don't use self.lock here.
+    #       * Do not call the public thread-safe methods here(with locking).
+    # These methods are called from the public thread-safe API, and will hang the process.
+
     def _create_update_index(self) -> Result[Ok, Err]:
         """Create or update mongo database indexes"""
         collection_status = self.collection
         if collection_status.is_err():
             return collection_status
         collection = collection_status.ok()
 
@@ -176,15 +184,15 @@
         if not hasattr(self, "_collection"):
             res = self.init_store()
             if res.is_err():
                 return res
 
         return Ok(self._collection)
 
-    def set(
+    def _set(
         self,
         obj: SyftObject,
         ignore_duplicates: bool = False,
     ) -> Result[SyftObject, str]:
         storage_obj = obj.to(self.storage_type)
 
         collection_status = self.collection
@@ -197,24 +205,24 @@
         try:
             collection.insert_one(storage_obj)
         except DuplicateKeyError as e:
             return Err(f"Duplicate Key Error for {obj}: {e}")
 
         return Ok(obj)
 
-    def update(self, qk: QueryKey, obj: SyftObject) -> Result[SyftObject, str]:
+    def _update(self, qk: QueryKey, obj: SyftObject) -> Result[SyftObject, str]:
         collection_status = self.collection
         if collection_status.is_err():
             return collection_status
         collection = collection_status.ok()
 
         # TODO: optimize the update. The ID should not be overwritten,
         # but the qk doesn't necessarily have to include the `id` field either.
 
-        prev_obj_status = self.get_all_from_store(QueryKeys(qks=[qk]))
+        prev_obj_status = self._get_all_from_store(QueryKeys(qks=[qk]))
         if prev_obj_status.is_err():
             return Err(f"No object found with query key: {qk}")
 
         prev_obj = prev_obj_status.ok()
         if len(prev_obj) == 0:
             return Err(f"Missing values for query key: {qk}")
 
@@ -233,52 +241,52 @@
         try:
             collection.update_one(filter=qk.as_dict_mongo, update={"$set": storage_obj})
         except Exception as e:
             return Err(f"Failed to update obj: {obj} with qk: {qk}. Error: {e}")
 
         return Ok(obj)
 
-    def find_index_or_search_keys(
+    def _find_index_or_search_keys(
         self, index_qks: QueryKeys, search_qks: QueryKeys
     ) -> Result[List[SyftObject], str]:
         # TODO: pass index as hint to find method
         qks = QueryKeys(qks=(index_qks.all + search_qks.all))
-        return self.get_all_from_store(qks=qks)
+        return self._get_all_from_store(qks=qks)
 
-    def get_all_from_store(self, qks: QueryKeys) -> Result[List[SyftObject], str]:
+    def _get_all_from_store(self, qks: QueryKeys) -> Result[List[SyftObject], str]:
         collection_status = self.collection
         if collection_status.is_err():
             return collection_status
         collection = collection_status.ok()
 
         storage_objs = collection.find(filter=qks.as_dict_mongo)
         syft_objs = []
         for storage_obj in storage_objs:
             obj = self.storage_type(storage_obj)
             transform_context = TransformContext(output={}, obj=obj)
             syft_objs.append(obj.to(self.settings.object_type, transform_context))
         return Ok(syft_objs)
 
-    def delete(self, qk: QueryKey) -> Result[SyftSuccess, Err]:
+    def _delete(self, qk: QueryKey) -> Result[SyftSuccess, Err]:
         collection_status = self.collection
         if collection_status.is_err():
             return collection_status
         collection = collection_status.ok()
 
         qks = QueryKeys(qks=qk)
         result = collection.delete_one(filter=qks.as_dict_mongo)
 
         if result.deleted_count == 1:
             return Ok(SyftSuccess(message="Deleted"))
 
         return Err(f"Failed to delete object with qk: {qk}")
 
-    def all(self):
+    def _all(self):
         qks = QueryKeys(qks=())
-        return self.get_all_from_store(qks=qks)
+        return self._get_all_from_store(qks=qks)
 
     def __len__(self):
         collection_status = self.collection
         if collection_status.is_err():
             return 0
         collection = collection_status.ok()
         return collection.count_documents(filter={})
@@ -303,12 +311,21 @@
     Parameters:
         `client_config`: MongoStoreClientConfig
             Mongo connection details: hostname, port, user, password etc.
         `store_type`: Type[DocumentStore]
             The type of the DocumentStore. Default: MongoDocumentStore
         `db_name`: str
             Database name
+        locking_config: LockingConfig
+            The config used for store locking. Available options:
+                * NoLockingConfig: no locking, ideal for single-thread stores.
+                * ThreadingLockingConfig: threading-based locking, ideal for same-process in-memory stores.
+                * FileLockingConfig: file based locking, ideal for same-device different-processes/threads stores.
+                * RedisLockingConfig: Redis-based locking, ideal for multi-device stores.
+            Defaults to NoLockingConfig.
     """
 
     client_config: MongoStoreClientConfig
     store_type: Type[DocumentStore] = MongoDocumentStore
     db_name: str = "app"
+    # TODO: should use a distributed lock, with RedisLockingConfig
+    locking_config: LockingConfig = NoLockingConfig()
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/network_service.py` & `syft-0.8.0b7/src/syft/core/node/new/network_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/node.py` & `syft-0.8.0b7/src/syft/core/node/new/node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/node_metadata.py` & `syft-0.8.0b7/src/syft/core/node/new/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/numpy.py` & `syft-0.8.0b7/src/syft/core/node/new/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/pandas.py` & `syft-0.8.0b7/src/syft/core/node/new/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/project.py` & `syft-0.8.0b7/src/syft/core/node/new/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/project_service.py` & `syft-0.8.0b7/src/syft/core/node/new/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/project_stash.py` & `syft-0.8.0b7/src/syft/core/node/new/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/queue_stash.py` & `syft-0.8.0b7/src/syft/core/node/new/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/recursive.py` & `syft-0.8.0b7/src/syft/core/node/new/recursive.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # stdlib
 from enum import Enum
 import sys
+import threading
 import types
 from typing import Any
 from typing import Callable
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
@@ -22,14 +23,18 @@
 from .capnp import get_capnp_schema
 
 TYPE_BANK = {}
 
 recursive_scheme = get_capnp_schema("recursive_serde.capnp").RecursiveSerde  # type: ignore
 
 
+def thread_ident() -> int:
+    return threading.current_thread().ident
+
+
 def recursive_serde_register(
     cls: Union[object, type],
     serialize: Optional[Callable] = None,
     deserialize: Optional[Callable] = None,
     serialize_attrs: Optional[List] = None,
     exclude_attrs: Optional[List] = None,
     inherit_attrs: Optional[bool] = True,
@@ -83,14 +88,15 @@
     # without fqn duplicate class names overwrite
     TYPE_BANK[fqn] = (
         nonrecursive,
         _serialize,
         _deserialize,
         attribute_list,
         serde_overrides,
+        cls,
     )
 
 
 def chunk_bytes(
     data: bytes, field_name: Union[str, int], builder: _DynamicStructBuilder
 ) -> None:
     CHUNK_SIZE = int(5.12e8)  # capnp max for a List(Data) field
@@ -121,14 +127,15 @@
     msg.fullyQualifiedName = fqn
     (
         nonrecursive,
         serialize,
         deserialize,
         attribute_list,
         serde_overrides,
+        cls,
     ) = TYPE_BANK[fqn]
 
     if nonrecursive:
         if serialize is None:
             raise Exception(
                 f"Cant serialize {type(self)} nonrecursive without serialize."
             )
@@ -175,28 +182,54 @@
 def rs_proto2object(proto: _DynamicStructBuilder) -> Any:
     # relative
     from .deserialize import _deserialize
 
     # clean this mess, Tudor
     module_parts = proto.fullyQualifiedName.split(".")
     klass = module_parts.pop()
-
     class_type: Type = type(None)
+
     if klass != "NoneType":
         try:
             class_type = index_syft_by_module_name(proto.fullyQualifiedName)  # type: ignore
         except Exception:  # nosec
-            class_type = getattr(sys.modules[".".join(module_parts)], klass)
+            try:
+                class_type = getattr(sys.modules[".".join(module_parts)], klass)
+            except Exception:  # nosec
+                if "syft.user" in proto.fullyQualifiedName:
+                    # relative
+                    from ..worker import CODE_RELOADER
+
+                    for _, load_user_code in CODE_RELOADER.items():
+                        load_user_code()
+                try:
+                    class_type = getattr(sys.modules[".".join(module_parts)], klass)
+                except Exception:  # nosec
+                    pass
 
     if proto.fullyQualifiedName not in TYPE_BANK:
-        raise Exception(f"{proto.fully_qualified_name} not in TYPE_BANK")
+        raise Exception(f"{proto.fullyQualifiedName} not in TYPE_BANK")
 
-    nonrecursive, serialize, deserialize, attribute_list, serde_overrides = TYPE_BANK[
-        proto.fullyQualifiedName
-    ]
+    # TODO: 🐉 sort this out, basically sometimes the syft.user classes are not in the
+    # module name space in sub-processes or threads even though they are loaded on start
+    # its possible that the uvicorn awsgi server is preloading a bunch of threads
+    # however simply getting the class from the TYPE_BANK doesn't always work and
+    # causes some errors so it seems like we want to get the local one where possible
+    (
+        nonrecursive,
+        serialize,
+        deserialize,
+        attribute_list,
+        serde_overrides,
+        cls,
+    ) = TYPE_BANK[proto.fullyQualifiedName]
+
+    if class_type == type(None):
+        # yes this looks stupid but it works and the opposite breaks
+        class_type = cls
 
     if nonrecursive:
         if deserialize is None:
             raise Exception(
                 f"Cant serialize {type(proto)} nonrecursive without serialize."
             )
 
@@ -217,15 +250,24 @@
         return getattr(class_type, "serde_constructor")(kwargs)
 
     if issubclass(class_type, Enum) and "value" in kwargs:
         obj = class_type.__new__(class_type, kwargs["value"])  # type: ignore
     elif issubclass(class_type, BaseModel):
         # if we skip the __new__ flow of BaseModel we get the error
         # AttributeError: object has no attribute '__fields_set__'
-        obj = class_type(**kwargs)
+
+        if "syft.user" in proto.fullyQualifiedName:
+            # weird issues with pydantic and ForwardRef on user classes being inited
+            # with custom state args / kwargs
+            obj = class_type()
+            for attr_name, attr_value in kwargs.items():
+                setattr(obj, attr_name, attr_value)
+        else:
+            obj = class_type(**kwargs)
+
     else:
         obj = class_type.__new__(class_type)  # type: ignore
         for attr_name, attr_value in kwargs.items():
             setattr(obj, attr_name, attr_value)
 
     return obj
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/recursive_primitives.py` & `syft-0.8.0b7/src/syft/core/node/new/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/request.py` & `syft-0.8.0b7/src/syft/core/node/new/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # stdlib
 from enum import Enum
 import hashlib
+import inspect
 from typing import Any
 from typing import Callable
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
 
@@ -149,19 +150,16 @@
         for change in self.changes:
             result = change.revert(context=change_context)
             if result.is_err():
                 return result
         return Ok(SyftSuccess(message=f"Request {self.id} changes reverted"))
 
     def accept_by_depositing_result(self, result: Any):
-        if len(self.changes) != 1:
-            raise Exception(
-                f"accept_by_depositing_result can only be run on {UserCode} Requests"
-            )
-
+        # this code is extremely brittle because its a work around that relies on
+        # the type of request being very specifically tied to code which needs approving
         change = self.changes[0]
         if not change.is_type(UserCode):
             raise Exception(
                 f"accept_by_depositing_result can only be run on {UserCode} not "
                 f"{change.linked_obj.object_type}"
             )
         if not type(change) == UserCodeStatusChange:
@@ -175,29 +173,33 @@
             raise Exception(f"Login to {self.node_uid} first.")
 
         action_object = ActionObject.from_obj(result)
         result = api.services.action.save(action_object)
         if not result:
             return result
 
+        permission_request = self.approve()
+        if not permission_request:
+            return permission_request
+
         code = change.linked_obj.resolve
-        state = code.output_policy_state
+        state = code.output_policy
         ctx = AuthedServiceContext(credentials=api.signing_key.verify_key)
-        state.update_state(outputs=action_object.id, context=ctx)
+
+        state.apply_output(context=ctx, outputs=action_object)
         policy_state_mutation = ObjectMutation(
             linked_obj=change.linked_obj,
-            attr_name="output_policy_state",
+            attr_name="output_policy",
             match_type=True,
             value=state,
         )
 
         action_object_link = LinkedObject.from_obj(
             action_object, node_uid=self.node_uid
         )
-
         permission_change = ActionStoreChange(
             linked_obj=action_object_link, apply_permission_type=ActionPermission.READ
         )
 
         submit_request = SubmitRequest(
             changes=[policy_state_mutation, permission_change],
             requesting_user_verify_key=self.requesting_user_verify_key,
@@ -275,15 +277,21 @@
     attr_name: str
     value: Optional[Any]
     match_type: bool
 
     __attr_repr_cols__ = ["linked_obj", "attr_name"]
 
     def mutate(self, obj: Any) -> Any:
-        setattr(obj, self.attr_name, self.value)
+        # check if attribute is a property setter first
+        # this seems necessary for pydantic types
+        attr = getattr(type(obj), self.attr_name, None)
+        if inspect.isdatadescriptor(attr):
+            attr.fset(obj, self.value)
+        else:
+            setattr(obj, self.attr_name, self.value)
         return obj
 
     def _run(
         self, context: ChangeContext, apply: bool
     ) -> Result[SyftSuccess, SyftError]:
         try:
             obj = self.linked_obj.resolve_with_context(context)
@@ -378,14 +386,15 @@
                 return Err(valid)
             obj = self.linked_obj.resolve_with_context(context)
             if obj.is_err():
                 return SyftError(message=obj.err())
             obj = obj.ok()
             if apply:
                 obj = self.mutate(obj)
+
                 self.linked_obj.update_with_context(context, obj)
             else:
                 raise NotImplementedError
             return Ok(SyftSuccess(message=f"{type(self)} Success"))
         except Exception as e:
             print(f"failed to apply {type(self)}. {e}")
             return Err(SyftError(message=e))
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/request_service.py` & `syft-0.8.0b7/src/syft/core/node/new/request_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/request_stash.py` & `syft-0.8.0b7/src/syft/core/node/new/request_stash.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from .credentials import SyftVerifyKey
 from .document_store import BaseUIDStoreStash
 from .document_store import PartitionKey
 from .document_store import PartitionSettings
 from .document_store import QueryKeys
 from .request import Request
 from .request import RequestStatus
-from .response import SyftError
 from .serializable import serializable
 
 RequestingUserVerifyKeyPartitionKey = PartitionKey(
     key="requesting_user_verify_key", type_=SyftVerifyKey
 )
 StatusPartitionKey = PartitionKey(key="status", type_=RequestStatus)
 
@@ -28,18 +27,16 @@
     object_type = Request
     settings: PartitionSettings = PartitionSettings(
         name=Request.__canonical_name__, object_type=Request
     )
 
     def get_all_for_verify_key(
         self, verify_key: RequestingUserVerifyKeyPartitionKey
-    ) -> Result[List[Request], SyftError]:
+    ) -> Result[List[Request], str]:
         if isinstance(verify_key, str):
             verify_key = SyftVerifyKey.from_string(verify_key)
         qks = QueryKeys(qks=[RequestingUserVerifyKeyPartitionKey.with_obj(verify_key)])
         return self.query_all(qks=qks)
 
-    def get_all_for_status(
-        self, status: RequestStatus
-    ) -> Result[List[Request], SyftError]:
+    def get_all_for_status(self, status: RequestStatus) -> Result[List[Request], str]:
         qks = QueryKeys(qks=[StatusPartitionKey.with_obj(status)])
         return self.query_all(qks=qks)
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/response.py` & `syft-0.8.0b7/src/syft/core/node/new/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/serializable.py` & `syft-0.8.0b7/src/syft/core/node/new/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/service.py` & `syft-0.8.0b7/src/syft/core/node/new/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import Union
 
+# third party
+from result import Ok
+from result import OkErr
+
 # relative
 from .context import AuthedServiceContext
 from .linked_obj import LinkedObject
 from .response import SyftError
 from .serializable import serializable
 from .signature import Signature
 from .signature import signature_remove_context
@@ -37,15 +41,22 @@
 class AbstractService:
     node: AbstractNode
     node_uid: UID
 
     def resolve_link(
         self, context: AuthedServiceContext, linked_obj: LinkedObject
     ) -> Union[Any, SyftError]:
-        return self.stash.get_by_uid(uid=linked_obj.object_uid)
+        obj = self.stash.get_by_uid(uid=linked_obj.object_uid)
+        if isinstance(obj, OkErr) and obj.is_ok():
+            obj = obj.ok()
+        if hasattr(obj, "node_uid"):
+            obj.node_uid = context.node.id
+        if not isinstance(obj, OkErr):
+            obj = Ok(obj)
+        return obj
 
 
 @serializable()
 class ServiceConfig(SyftBaseObject):
     public_path: str
     private_path: str
     public_name: str
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/signature.py` & `syft-0.8.0b7/src/syft/core/node/new/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/sqlite_document_store.py` & `syft-0.8.0b7/src/syft/core/node/new/sqlite_document_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from .deserialize import _deserialize
 from .document_store import DocumentStore
 from .document_store import PartitionSettings
 from .document_store import StoreClientConfig
 from .document_store import StoreConfig
 from .kv_document_store import KeyValueBackingStore
 from .kv_document_store import KeyValueStorePartition
+from .locks import FileLockingConfig
+from .locks import LockingConfig
 from .serializable import serializable
 from .serialize import _serialize
 from .uid import UID
 
 
 def _repr_debug_(value: Any) -> str:
     if hasattr(value, "_repr_debug_"):
@@ -83,14 +85,15 @@
         self.file_path = self.store_config.client_config.file_path
         self._db[thread_ident()] = sqlite3.connect(
             self.file_path,
             timeout=self.store_config.client_config.timeout,
             check_same_thread=self.store_config.client_config.check_same_thread,
         )
 
+        # TODO: Review OSX compatibility.
         # Set journal mode to WAL.
         # self._db[thread_ident()].execute("pragma journal_mode=wal")
 
     def create_table(self):
         try:
             self.cur.execute(
                 f"create table {self.table_name} (uid VARCHAR(32) NOT NULL PRIMARY KEY, "  # nosec
@@ -146,53 +149,70 @@
     def _update(self, key: UID, value: Any) -> None:
         insert_sql = f"update {self.table_name} set uid = ?, repr = ?, value = ? where uid = ?"  # nosec
         data = _serialize(value, to_bytes=True)
         self._execute(insert_sql, [str(key), _repr_debug_(value), data, str(key)])
 
     def _get(self, key: UID) -> Any:
         select_sql = f"select * from {self.table_name} where uid = ?"  # nosec
-        row = self._execute(select_sql, [str(key)]).fetchone()
+        cursor = self._execute(select_sql, [str(key)])
+        if cursor is None:
+            raise KeyError(f"Query {select_sql} failed")
+
+        row = cursor.fetchone()
         if row is None or len(row) == 0:
             raise KeyError(f"{key} not in {type(self)}")
         data = row[2]
         return _deserialize(data, from_bytes=True)
 
     def _exists(self, key: UID) -> bool:
         select_sql = f"select uid from {self.table_name} where uid = ?"  # nosec
-        row = self._execute(select_sql, [str(key)]).fetchone()
+
+        cursor = self._execute(select_sql, [str(key)])
+        if cursor is None:
+            return False
+
+        row = cursor.fetchone()
         if row is None:
             return False
+
         return bool(row)
 
     def _get_all(self) -> Any:
         select_sql = f"select * from {self.table_name}"  # nosec
         keys = []
         data = []
-        rows = self._execute(select_sql).fetchall()
 
+        cursor = self._execute(select_sql)
+        if cursor is None:
+            return {}
+
+        rows = cursor.fetchall()
         if rows is None:
             return {}
 
         for row in rows:
             keys.append(UID(row[0]))
             data.append(_deserialize(row[2], from_bytes=True))
         return dict(zip(keys, data))
 
     def _get_all_keys(self) -> Any:
-        try:
-            select_sql = f"select uid from {self.table_name}"  # nosec
-            keys = []
-            rows = self._execute(select_sql).fetchall()
-            if rows is None:
-                return []
-            for row in rows:
-                keys.append(UID(row[0]))
-            return keys
-        except Exception as e:
-            raise e
+        select_sql = f"select uid from {self.table_name}"  # nosec
+        keys = []
+
+        cursor = self._execute(select_sql)
+        if cursor is None:
+            return []
+
+        rows = cursor.fetchall()
+        if rows is None:
+            return []
+
+        for row in rows:
+            keys.append(UID(row[0]))
+        return keys
 
     def _delete(self, key: UID) -> None:
         select_sql = f"delete from {self.table_name} where uid = ?"  # nosec
         self._execute(select_sql, [str(key)])
 
     def _delete_all(self) -> None:
         select_sql = f"delete from {self.table_name}"  # nosec
@@ -236,14 +256,15 @@
     def values(self) -> Any:
         return self._get_all().values()
 
     def items(self) -> Any:
         return self._get_all().items()
 
     def pop(self, key: Any) -> Self:
+        # NOTE: not thread-safe
         value = self._get(key)
         self._delete(key)
         return value
 
     def __contains__(self, key: Any) -> bool:
         return self._exists(key)
 
@@ -265,22 +286,32 @@
         `settings`: PartitionSettings
             PySyft specific settings, used for indexing and partitioning
         `store_config`: SQLiteStoreConfig
             SQLite specific configuration
     """
 
     def close(self) -> None:
-        self.data._close()
-        self.unique_keys._close()
-        self.searchable_keys._close()
+        self.lock.acquire()
+        try:
+            self.data._close()
+            self.unique_keys._close()
+            self.searchable_keys._close()
+        except BaseException:
+            pass
+        self.lock.release()
 
     def commit(self) -> None:
-        self.data._commit()
-        self.unique_keys._commit()
-        self.searchable_keys._commit()
+        self.lock.acquire()
+        try:
+            self.data._commit()
+            self.unique_keys._commit()
+            self.searchable_keys._commit()
+        except BaseException:
+            pass
+        self.lock.release()
 
 
 # the base document store is already a dict but we can change it later
 @serializable()
 class SQLiteDocumentStore(DocumentStore):
     """SQLite Document Store
 
@@ -339,12 +370,20 @@
     Parameters:
         `client_config`: SQLiteStoreClientConfig
             SQLite connection configuration
         `store_type`: DocumentStore
             Class interacting with QueueStash. Default: SQLiteDocumentStore
         `backing_store`: KeyValueBackingStore
             The Store core logic. Default: SQLiteBackingStore
+        locking_config: LockingConfig
+            The config used for store locking. Available options:
+                * NoLockingConfig: no locking, ideal for single-thread stores.
+                * ThreadingLockingConfig: threading-based locking, ideal for same-process in-memory stores.
+                * FileLockingConfig: file based locking, ideal for same-device different-processes/threads stores.
+                * RedisLockingConfig: Redis-based locking, ideal for multi-device stores.
+            Defaults to FileLockingConfig.
     """
 
     client_config: SQLiteStoreClientConfig
     store_type: Type[DocumentStore] = SQLiteDocumentStore
     backing_store: Type[KeyValueBackingStore] = SQLiteBackingStore
+    locking_config: LockingConfig = FileLockingConfig()
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/syft_object.py` & `syft-0.8.0b7/src/syft/core/node/new/syft_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,31 @@
     __object_transform_registry__: Dict[str, Callable] = {}
 
     def __init_subclass__(cls, **kwargs: Any) -> None:
         super().__init_subclass__(**kwargs)
         if hasattr(cls, "__canonical_name__") and hasattr(cls, "__version__"):
             mapping_string = f"{cls.__canonical_name__}_{cls.__version__}"
             if mapping_string in cls.__object_version_registry__:
-                raise Exception(f"Duplicate mapping for {mapping_string} and {cls}")
-            cls.__object_version_registry__[mapping_string] = cls
+                current_cls = cls.__object_version_registry__[mapping_string]
+                if cls == current_cls:
+                    # same class so noop
+                    return None
+
+                # user code is reinitialized which means it might have a new address
+                # in memory so for that we can just skip
+                if "syft.user" in cls.__module__:
+                    # this happens every time we reload the user code
+                    return None
+                else:
+                    # this shouldn't happen and is usually a mistake of reusing the
+                    # same __canonical_name__ and __version__ in two classes
+                    raise Exception(f"Duplicate mapping for {mapping_string} and {cls}")
+            else:
+                # only if the cls has not been registered do we want to register it
+                cls.__object_version_registry__[mapping_string] = cls
 
     @classmethod
     def versioned_class(cls, name: str, version: int) -> Optional[Type["SyftObject"]]:
         mapping_string = f"{name}_{version}"
         if mapping_string not in cls.__object_version_registry__:
             return None
         return cls.__object_version_registry__[mapping_string]
@@ -129,15 +144,14 @@
     @pydantic.root_validator(pre=True)
     def make_id(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         id_field = cls.__fields__["id"]
         if "id" not in values and id_field.required:
             values["id"] = id_field.type_()
         return values
 
-    __attr_state__: List[str]  # persistent recursive serde keys
     __attr_searchable__: List[str] = []  # keys which can be searched in the ORM
     __attr_unique__: List[str] = []
     # the unique keys for the particular Collection the objects will be stored in
     __serde_overrides__: Dict[
         str, Sequence[Callable]
     ] = {}  # List of attributes names which require a serde override.
     __owner__: str
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/test_service.py` & `syft-0.8.0b7/src/syft/core/node/new/test_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/third_party.py` & `syft-0.8.0b7/src/syft/core/node/new/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/transforms.py` & `syft-0.8.0b7/src/syft/core/node/new/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/twin_object.py` & `syft-0.8.0b7/src/syft/core/node/new/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/uid.py` & `syft-0.8.0b7/src/syft/core/node/new/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/user.py` & `syft-0.8.0b7/src/syft/core/node/new/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/user_code.py` & `syft-0.8.0b7/src/syft/core/node/new/policy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,121 +1,196 @@
 # future
 from __future__ import annotations
 
 # stdlib
 import ast
+from copy import deepcopy
 from enum import Enum
 import hashlib
 import inspect
 from inspect import Parameter
 from inspect import Signature
 from io import StringIO
 import sys
+import types
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
-from typing import Type
 from typing import Union
 
 # third party
-import astunparse  # ast.unparse for python 3.8
-from result import Err
+from RestrictedPython import compile_restricted
 from result import Ok
-from result import Result
 
 # relative
+from ....util import is_interpreter_jupyter
+from .action_object import ActionObject
 from .api import NodeView
+from .code_parse import GlobalsVisitor
 from .context import AuthedServiceContext
 from .context import NodeServiceContext
 from .credentials import SyftVerifyKey
 from .dataset import Asset
 from .datetime import DateTime
 from .document_store import PartitionKey
 from .node import NodeType
-from .node_metadata import EnclaveMetadata
 from .response import SyftError
 from .response import SyftSuccess
 from .serializable import serializable
 from .syft_object import SYFT_OBJECT_VERSION_1
 from .syft_object import SyftObject
 from .transforms import TransformContext
 from .transforms import generate_id
 from .transforms import transform
+from .twin_object import TwinObject
 from .uid import UID
-from .user_code_parse import GlobalsVisitor
-
-UserVerifyKeyPartitionKey = PartitionKey(key="user_verify_key", type_=SyftVerifyKey)
-CodeHashPartitionKey = PartitionKey(key="code_hash", type_=int)
+from .unparse import unparse
 
+PolicyUserVerifyKeyPartitionKey = PartitionKey(
+    key="user_verify_key", type_=SyftVerifyKey
+)
 PyCodeObject = Any
 
 
-class InputPolicy(SyftObject):
+def extract_uid(v: Any) -> UID:
+    value = v
+    if isinstance(v, ActionObject):
+        value = v.id
+    if isinstance(v, TwinObject):
+        value = v.id
+
+    if not isinstance(value, UID):
+        raise Exception(f"Input {v} must have a UID not {type(v)}")
+    return value
+
+
+def filter_only_uids(results: Any) -> Dict[str, Any]:
+    if not hasattr(results, "__len__"):
+        results = [results]
+
+    if isinstance(results, list):
+        output_list = []
+        for v in results:
+            output_list.append(extract_uid(v))
+        return output_list
+    elif isinstance(results, dict):
+        output_dict = {}
+        for k, v in results.items():
+            output_dict[k] = extract_uid(v)
+        return output_dict
+    return extract_uid(results)
+
+
+class Policy(SyftObject):
     # version
-    __canonical_name__ = "InputPolicy"
+    __canonical_name__ = "Policy"
     __version__ = SYFT_OBJECT_VERSION_1
 
+    id: UID
+    init_kwargs: Dict[Any, Any] = {}
+
+    def __init__(self, *args, **kwargs) -> None:
+        if "init_kwargs" in kwargs:
+            init_kwargs = kwargs["init_kwargs"]
+            del kwargs["init_kwargs"]
+        else:
+            init_kwargs = deepcopy(kwargs)
+            if "id" in init_kwargs:
+                del init_kwargs["id"]
+        super().__init__(init_kwargs=init_kwargs, *args, **kwargs)
+
+    @classmethod
+    @property
+    def policy_code(cls) -> str:
+        mro = reversed(cls.mro())
+        op_code = ""
+        for klass in mro:
+            if "Policy" in klass.__name__:
+                op_code += inspect.getsource(klass)
+                op_code += "\n"
+        return op_code
+
+    def public_state() -> None:
+        raise NotImplementedError
+
+    @property
+    def valid(self) -> Union[SyftSuccess, SyftError]:
+        return SyftSuccess(message="Policy is valid.")
+
+
+@serializable()
+class UserPolicyStatus(Enum):
+    SUBMITTED = "submitted"
+    DENIED = "denied"
+    APPROVED = "approved"
+
+
+def partition_by_node(kwargs: Dict[str, Any]) -> Dict[str, UID]:
     # relative
+    from .action_object import ActionObject
+    from .api import APIRegistry
     from .api import NodeView
+    from .twin_object import TwinObject
 
-    id: UID
-    inputs: Dict[NodeView, Any]
-    node_uid: Optional[UID]
+    # fetches the all the current api's connected
+    api_list = APIRegistry.get_all_api()
+    output_kwargs = {}
+    for k, v in kwargs.items():
+        uid = v
+        if isinstance(v, ActionObject):
+            uid = v.id
+        if isinstance(v, TwinObject):
+            uid = v.id
+        if isinstance(v, Asset):
+            uid = v.action_id
+
+        if not isinstance(uid, UID):
+            raise Exception(f"Input {k} must have a UID not {type(v)}")
+
+        _obj_exists = False
+        for api in api_list:
+            if api.services.action.exists(uid):
+                node_view = NodeView.from_api(api)
+                if node_view not in output_kwargs:
+                    output_kwargs[node_view] = {k: uid}
+                else:
+                    output_kwargs[node_view].update({k: uid})
+
+                _obj_exists = True
+                break
+
+        if not _obj_exists:
+            raise Exception(f"Input data {k}:{uid} does not belong to any Domain")
+
+    return output_kwargs
+
+
+class InputPolicy(Policy):
+    __canonical_name__ = "InputPolicy"
+    __version__ = SYFT_OBJECT_VERSION_1
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
-        # TODO: This method initialization would conflict if one of the input variables
-        # to the code submission function happens to be id or inputs
-        uid = UID()
-        node_uid = None
-        if "id" in kwargs:
-            uid = kwargs["id"]
-        if "node_uid" in kwargs:
-            node_uid = kwargs["node_uid"]
-
-        # finally get inputs
-        if "inputs" in kwargs:
-            kwargs = kwargs["inputs"]
+        if "init_kwargs" in kwargs:
+            init_kwargs = kwargs["init_kwargs"]
+            del kwargs["init_kwargs"]
         else:
-            kwargs = partition_by_node(kwargs)
-        super().__init__(id=uid, inputs=kwargs, node_uid=node_uid)
+            # TODO: remove this tech debt
+            init_kwargs = partition_by_node(kwargs)
+        super().__init__(*args, init_kwargs=init_kwargs, **kwargs)
 
-    def filter_kwargs(kwargs: Dict[str, Any]) -> Dict[str, Any]:
+    def filter_kwargs(
+        self, kwargs: Dict[Any, Any], context: AuthedServiceContext, code_item_id: UID
+    ) -> Dict[Any, Any]:
         raise NotImplementedError
 
-    def __getitem__(self, key: Union[int, str]) -> Optional[SyftObject]:
-        if isinstance(key, int):
-            key = list(self.inputs.keys())[key]
-        uid = self.inputs[key]
-        # TODO Add NODE UID or LINK so we can resolve this object
-        return uid
-
     @property
-    def assets(self) -> List[Asset]:
-        # relative
-        from .api import APIRegistry
-
-        api = APIRegistry.api_for(self.node_uid)
-        if api is None:
-            return SyftError(message=f"You must login to {self.node_uid}")
-
-        node_view = NodeView(
-            node_name=api.node_name, verify_key=api.signing_key.verify_key
-        )
-        inputs = self.inputs[node_view]
-        all_assets = []
-        for k, uid in inputs.items():
-            if isinstance(uid, UID):
-                assets = api.services.dataset.get_assets_by_action_id(uid)
-                if not isinstance(assets, list):
-                    return assets
-
-                all_assets += assets
-        return all_assets
+    def inputs(self) -> Dict[NodeView, Any]:
+        return self.init_kwargs
 
 
 def retrieve_from_db(
     code_item_id: UID, allowed_inputs: Dict[str, UID], context: AuthedServiceContext
 ) -> Dict:
     # relative
     from .action_service import TwinMode
@@ -188,599 +263,455 @@
 @serializable()
 class ExactMatch(InputPolicy):
     # version
     __canonical_name__ = "ExactMatch"
     __version__ = SYFT_OBJECT_VERSION_1
 
     def filter_kwargs(
-        self, kwargs: Dict[str, Any], context: AuthedServiceContext, code_item_id: UID
-    ) -> Dict[str, Any]:
+        self, kwargs: Dict[Any, Any], context: AuthedServiceContext, code_item_id: UID
+    ) -> Dict[Any, Any]:
         allowed_inputs = allowed_ids_only(
             allowed_inputs=self.inputs, kwargs=kwargs, context=context
         )
-        return retrieve_from_db(
+        results = retrieve_from_db(
             code_item_id=code_item_id, allowed_inputs=allowed_inputs, context=context
         )
+        return results
 
 
 @serializable()
 class OutputHistory(SyftObject):
     # version
     __canonical_name__ = "OutputHistory"
     __version__ = SYFT_OBJECT_VERSION_1
 
     output_time: DateTime
     outputs: Optional[Union[List[UID], Dict[str, UID]]]
     executing_user_verify_key: SyftVerifyKey
 
 
-class OutputPolicyState(SyftObject):
+class OutputPolicy(Policy):
     # version
-    __canonical_name__ = "OutputPolicyState"
+    __canonical_name__ = "OutputPolicy"
     __version__ = SYFT_OBJECT_VERSION_1
 
     output_history: List[OutputHistory] = []
+    output_kwargs: List[str] = []
+    node_uid: Optional[UID]
 
-    @property
-    def valid(self) -> Union[SyftSuccess, SyftError]:
-        raise NotImplementedError
+    def apply_output(
+        self,
+        context: NodeServiceContext,
+        outputs: Any,
+    ) -> Any:
+        output_uids = filter_only_uids(outputs)
+        if isinstance(output_uids, UID):
+            output_uids = [output_uids]
+        history = OutputHistory(
+            output_time=DateTime.now(),
+            outputs=output_uids,
+            executing_user_verify_key=context.credentials,
+        )
+        self.output_history.append(history)
+        return outputs
 
-    def update_state(self) -> None:
-        raise NotImplementedError
+    @property
+    def outputs(self) -> List[str]:
+        return self.output_kwargs
 
 
 @serializable()
-class OutputPolicyStateExecuteCount(OutputPolicyState):
-    # version
-    __canonical_name__ = "OutputPolicyStateExecuteCount"
+class OutputPolicyExecuteCount(OutputPolicy):
+    __canonical_name__ = "OutputPolicyExecuteCount"
     __version__ = SYFT_OBJECT_VERSION_1
 
     count: int = 0
     limit: int
 
+    def apply_output(
+        self,
+        context: NodeServiceContext,
+        outputs: Any,
+    ) -> Optional[Any]:
+        if self.count < self.limit:
+            super().apply_output(context, outputs)
+            self.count += 1
+            return outputs
+        return None
+
     @property
     def valid(self) -> Union[SyftSuccess, SyftError]:
         is_valid = self.count < self.limit
         if is_valid:
             return SyftSuccess(
                 message=f"Policy is still valid. count: {self.count} < limit: {self.limit}"
             )
         return SyftError(
             message=f"Policy is no longer valid. count: {self.count} >= limit: {self.limit}"
         )
 
-    def update_state(
-        self,
-        context: NodeServiceContext,
-        outputs: Optional[Union[UID, List[UID], Dict[str, UID]]],
-    ) -> None:
-        if self.count >= self.limit:
-            raise Exception(
-                f"Update state being called with count: {self.count} "
-                f"beyond execution limit: {self.limit}"
-            )
-        if isinstance(outputs, UID):
-            outputs = [outputs]
-        history = OutputHistory(
-            output_time=DateTime.now(),
-            outputs=outputs,
-            executing_user_verify_key=context.credentials,
-        )
-        self.output_history.append(history)
-        self.count += 1
+    def public_state(self) -> None:
+        return {"limit": self.limit, "count": self.count}
 
 
 @serializable()
-class OutputPolicyStateExecuteOnce(OutputPolicyStateExecuteCount):
-    __canonical_name__ = "OutputPolicyStateExecuteOnce"
+class OutputPolicyExecuteOnce(OutputPolicyExecuteCount):
+    __canonical_name__ = "OutputPolicyExecuteOnce"
     __version__ = SYFT_OBJECT_VERSION_1
 
     limit: int = 1
 
 
-class OutputPolicy(SyftObject):
-    # version
-    __canonical_name__ = "OutputPolicy"
-    __version__ = SYFT_OBJECT_VERSION_1
+SingleExecutionExactOutput = OutputPolicyExecuteOnce
 
-    id: UID
-    outputs: List[str] = []
-    state_type: Optional[Type[OutputPolicyState]]
 
-    def update() -> None:
-        raise NotImplementedError
+class CustomPolicy(type):
+    # capture the init_kwargs transparently
+    def __call__(cls, *args: Any, **kwargs: Any) -> None:
+        obj = super().__call__(*args, **kwargs)
+        setattr(obj, "init_kwargs", kwargs)
+        return obj
 
-    @property
-    def policy_code(self) -> str:
-        cls = type(self)
-        op_code = inspect.getsource(cls)
-        if self.state_type:
-            state_code = inspect.getsource(self.state_type)
-            op_code += "\n" + state_code
-        return op_code
 
+class CustomOutputPolicy(metaclass=CustomPolicy):
+    def apply_output(
+        self,
+        context: NodeServiceContext,
+        outputs: Any,
+    ) -> Optional[Any]:
+        return outputs
 
-@serializable()
-class SingleExecutionExactOutput(OutputPolicy):
-    # version
-    __canonical_name__ = "SingleExecutionExactOutput"
-    __version__ = SYFT_OBJECT_VERSION_1
 
-    state_type: Type[OutputPolicyState] = OutputPolicyStateExecuteOnce
+class UserOutputPolicy(OutputPolicy):
+    __canonical_name__ = "UserOutputPolicy"
+    pass
 
 
-@serializable()
-class UserCodeStatus(Enum):
-    SUBMITTED = "submitted"
-    DENIED = "denied"
-    EXECUTE = "execute"
+class UserInputPolicy(InputPolicy):
+    __canonical_name__ = "UserInputPolicy"
+    pass
 
-    def __hash__(self) -> int:
-        return hash(self.value)
 
-
-# User Code status context for multiple approvals
-# To make nested dicts hashable for mongodb
-# as status is in attr_searchable
-@serializable(attrs=["base_dict"])
-class UserCodeStatusContext:
-    base_dict: Dict = {}
-
-    def __init__(self, base_dict: Dict):
-        self.base_dict = base_dict
-
-    def __repr__(self):
-        return str(self.base_dict)
-
-    def __hash__(self) -> int:
-        hash_sum = 0
-        for k, v in self.base_dict.items():
-            hash_sum = hash(k) + hash(v)
-        return hash_sum
-
-    def for_context(self, context: AuthedServiceContext) -> UserCodeStatus:
-        if context.node.node_type == NodeType.ENCLAVE:
-            keys = set(self.base_dict.values())
-            if len(keys) == 1 and UserCodeStatus.EXECUTE in keys:
-                return UserCodeStatus.EXECUTE
-            elif UserCodeStatus.SUBMITTED in keys and UserCodeStatus.DENIED not in keys:
-                return UserCodeStatus.SUBMITTED
-            elif UserCodeStatus.DENIED in keys:
-                return UserCodeStatus.DENIED
-            else:
-                return Exception(f"Invalid types in {keys} for Code Submission")
-
-        elif context.node.node_type == NodeType.DOMAIN:
-            node_view = NodeView(
-                node_name=context.node.name,
-                verify_key=context.node.signing_key.verify_key,
-            )
-            if node_view in self.base_dict:
-                return self.base_dict[node_view]
-            else:
-                raise Exception(
-                    f"Code Object does not contain {context.node.name} Domain's data"
-                )
-        else:
-            raise Exception(
-                f"Invalid Node Type for Code Submission:{context.node.node_type}"
-            )
-
-    def mutate(
-        self, value: UserCodeStatus, node_name: str, verify_key: SyftVerifyKey
-    ) -> Result[Ok, Err]:
-        node_view = NodeView(node_name=node_name, verify_key=verify_key)
-        base_dict = self.base_dict
-        if node_view in base_dict:
-            base_dict[node_view] = value
-            setattr(self, "base_dict", base_dict)
-            return Ok(self)
-        else:
-            return Err(
-                "Cannot Modify Status as the Domain's data is not included in the request"
-            )
+class CustomInputPolicy(metaclass=CustomPolicy):
+    pass
 
 
 @serializable()
-class UserCode(SyftObject):
-    # version
-    __canonical_name__ = "UserCode"
+class UserPolicy(Policy):
+    __canonical_name__ = "UserPolicy"
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: UID
+    node_uid: Optional[UID]
     user_verify_key: SyftVerifyKey
     raw_code: str
-    input_policy: InputPolicy
-    output_policy: OutputPolicy
-    output_policy_state: OutputPolicyState
     parsed_code: str
-    service_func_name: str
-    unique_func_name: str
-    user_unique_func_name: str
-    code_hash: str
     signature: inspect.Signature
-    status: UserCodeStatusContext
-    enclave_metadata: Optional[EnclaveMetadata] = None
-
-    __attr_searchable__ = ["user_verify_key", "status", "service_func_name"]
-    __attr_unique__ = ["code_hash", "user_unique_func_name"]
-    __attr_repr_cols__ = ["status", "service_func_name"]
+    class_name: str
+    unique_name: str
+    code_hash: str
+    byte_code: PyCodeObject
+    status: UserPolicyStatus = UserPolicyStatus.SUBMITTED
 
     @property
     def byte_code(self) -> Optional[PyCodeObject]:
         return compile_byte_code(self.parsed_code)
 
     @property
-    def unsafe_function(self) -> Optional[Callable]:
-        print("WARNING: This code was submitted by a User and could be UNSAFE.")
-
-        # 🟡 TODO: re-use the same infrastructure as the execute_byte_code function
-        def wrapper(*args: Any, **kwargs: Any) -> Callable:
-            # remove the decorator
-            inner_function = ast.parse(self.raw_code).body[0]
-            inner_function.decorator_list = []
-            # compile the function
-            raw_byte_code = compile_byte_code(astunparse.unparse(inner_function))
-            # load it
-            exec(raw_byte_code)  # nosec
-            # execute it
-            evil_string = f"{self.service_func_name}(*args, **kwargs)"
-            result = eval(evil_string, None, locals())  # nosec
-            # return the results
-            return result
-
-        return wrapper
-
-    @property
-    def code(self) -> str:
+    def policy_code(self) -> str:
         return self.raw_code
 
+    def apply_output(
+        self,
+        context: NodeServiceContext,
+        outputs: Any,
+    ) -> Optional[Any]:
+        return outputs
+
+
+def new_getfile(object):
+    if not inspect.isclass(object):
+        return inspect.getfile(object)
+
+    # Lookup by parent module (as in current inspect)
+    if hasattr(object, "__module__"):
+        object_ = sys.modules.get(object.__module__)
+        if hasattr(object_, "__file__"):
+            return object_.__file__
+
+    # If parent module is __main__, lookup by methods (NEW)
+    for _, member in inspect.getmembers(object):
+        if (
+            inspect.isfunction(member)
+            and object.__qualname__ + "." + member.__name__ == member.__qualname__
+        ):
+            return inspect.getfile(member)
+    else:
+        raise TypeError("Source for {!r} not found".format(object))
 
-def partition_by_node(kwargs: Dict[str, Any]) -> Dict[str, UID]:
-    # relative
-    from .action_object import ActionObject
-    from .api import APIRegistry
-    from .api import NodeView
-    from .twin_object import TwinObject
-
-    # fetches the all the current api's connected
-    api_list = APIRegistry.get_all_api()
-    output_kwargs = {}
-    for k, v in kwargs.items():
-        uid = v
-        if isinstance(v, ActionObject):
-            uid = v.id
-        if isinstance(v, TwinObject):
-            uid = v.id
-        if isinstance(v, Asset):
-            uid = v.action_id
-
-        if not isinstance(uid, UID):
-            raise Exception(f"Input {k} must have a UID not {type(v)}")
-
-        _obj_exists = False
-        for api in api_list:
-            if api.services.action.exists(uid):
-                node_view = NodeView.from_api(api)
-                if node_view not in output_kwargs:
-                    output_kwargs[node_view] = {k: uid}
-                else:
-                    output_kwargs[node_view].update({k: uid})
-
-                _obj_exists = True
-                break
 
-        if not _obj_exists:
-            raise Exception(f"Input data {k}:{uid} does not belong to any Domain")
+def get_code_from_class(policy):
+    klasses = [inspect.getmro(policy)[0]]  #
+    whole_str = ""
+    for klass in klasses:
+        if is_interpreter_jupyter():
+            # third party
+            from IPython.core.magics.code import extract_symbols
 
-    return output_kwargs
+            cell_code = "".join(inspect.linecache.getlines(new_getfile(klass)))
+            class_code = extract_symbols(cell_code, klass.__name__)[0][0]
+        else:
+            class_code = inspect.getsource(klass)
+        whole_str += class_code
+    return whole_str
 
 
 @serializable()
-class SubmitUserCode(SyftObject):
-    # version
-    __canonical_name__ = "SubmitUserCode"
+class SubmitUserPolicy(Policy):
+    __canonical_name__ = "SubmitUserPolicy"
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: Optional[UID]
     code: str
-    func_name: str
-    signature: inspect.Signature
-    input_policy: InputPolicy
-    output_policy: OutputPolicy
-    local_function: Optional[Callable]
-    enclave_metadata: Optional[EnclaveMetadata] = None
-
-    @property
-    def kwargs(self) -> List[str]:
-        return self.input_policy.inputs
-
-    @property
-    def outputs(self) -> List[str]:
-        return self.output_policy.outputs
+    class_name: str
+    input_kwargs: List[str]
 
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        # only run this on the client side
-        if self.local_function:
-            # filtered_args = []
-            filtered_kwargs = {}
-            # for arg in args:
-            #     filtered_args.append(debox_asset(arg))
-            for k, v in kwargs.items():
-                filtered_kwargs[k] = debox_asset(v)
+    def compile(self) -> PyCodeObject:
+        return compile_restricted(self.code, "<string>", "exec")
 
-            return self.local_function(**filtered_kwargs)
-        else:
-            raise NotImplementedError
-
-
-def debox_asset(arg: Any) -> Any:
-    deboxed_arg = arg
-    if isinstance(deboxed_arg, Asset):
-        deboxed_arg = arg.mock
-    if hasattr(deboxed_arg, "syft_action_data"):
-        deboxed_arg = deboxed_arg.syft_action_data
-    return deboxed_arg
-
-
-def syft_function(input_policy, output_policy) -> SubmitUserCode:
-    def decorator(f):
-        return SubmitUserCode(
-            code=inspect.getsource(f),
-            func_name=f.__name__,
-            signature=inspect.signature(f),
-            input_policy=input_policy,
-            output_policy=output_policy,
-            local_function=f,
+    @staticmethod
+    def from_obj(policy_obj: CustomPolicy) -> SubmitUserPolicy:
+        user_class = policy_obj.__class__
+        init_f_code = user_class.__init__.__code__
+        return SubmitUserPolicy(
+            code=get_code_from_class(user_class),
+            class_name=user_class.__name__,
+            input_kwargs=init_f_code.co_varnames[1 : init_f_code.co_argcount],
         )
 
-    return decorator
 
+def hash_code(context: TransformContext) -> TransformContext:
+    code = context.output["code"]
+    del context.output["code"]
+    context.output["raw_code"] = code
+    code_hash = hashlib.sha256(code.encode("utf8")).hexdigest()
+    context.output["code_hash"] = code_hash
+    return context
 
-def generate_unique_func_name(context: TransformContext) -> TransformContext:
+
+def generate_unique_class_name(context: TransformContext) -> TransformContext:
+    # TODO: Do we need to check if the initial name contains underscores?
     code_hash = context.output["code_hash"]
-    service_func_name = context.output["func_name"]
-    context.output["service_func_name"] = service_func_name
-    func_name = f"user_func_{service_func_name}_{context.credentials}_{code_hash}"
-    user_unique_func_name = f"user_func_{service_func_name}_{context.credentials}"
-    context.output["unique_func_name"] = func_name
-    context.output["user_unique_func_name"] = user_unique_func_name
+    service_class_name = context.output["class_name"]
+    unique_name = f"{service_class_name}_{context.credentials}_{code_hash}"
+    context.output["unique_name"] = unique_name
     return context
 
 
-def process_code(
-    raw_code: str,
-    func_name: str,
-    original_func_name: str,
-    input_policy: InputPolicy,
-    output_policy: OutputPolicy,
-) -> str:
-    input_kwargs = input_policy.inputs
-    outputs = output_policy.outputs
+def compile_byte_code(parsed_code: str) -> Optional[PyCodeObject]:
+    try:
+        return compile(parsed_code, "<string>", "exec")
+    except Exception as e:
+        print("WARNING: to compile byte code", e)
+    return None
+
 
+def process_class_code(raw_code: str, class_name: str) -> str:
     tree = ast.parse(raw_code)
-
-    # check there are no globals
     v = GlobalsVisitor()
     v.visit(tree)
+    if len(tree.body) != 1 or not isinstance(tree.body[0], ast.ClassDef):
+        raise Exception(
+            "Class code should only contain the Class definition for your policy"
+        )
+    old_class = tree.body[0]
+    if len(old_class.bases) != 1 or old_class.bases[0].attr not in [
+        CustomInputPolicy.__name__,
+        CustomOutputPolicy.__name__,
+    ]:
+        raise Exception(
+            f"Class code should either implement {CustomInputPolicy.__name__} "
+            f"or {CustomOutputPolicy.__name__}"
+        )
 
-    f = tree.body[0]
-    f.decorator_list = []
+    # TODO: changes the bases
+    old_class.bases[0].attr = old_class.bases[0].attr.replace("Custom", "User")
 
-    keywords = [
-        ast.keyword(arg=i, value=[ast.Name(id=i)])
-        for _, inputs in input_kwargs.items()
-        for i in inputs
-    ]
-    call_stmt = ast.Assign(
-        targets=[ast.Name(id="result")],
-        value=ast.Call(
-            func=ast.Name(id=original_func_name), args=[], keywords=keywords
-        ),
-        lineno=0,
+    serializable_name = ast.Name(id="sy.serializable", ctx=ast.Load())
+    serializable_decorator = ast.Call(
+        func=serializable_name,
+        args=[],
+        keywords=[],
     )
 
-    if len(outputs) > 0:
-        output_list = ast.List(elts=[ast.Constant(value=x) for x in outputs])
-        return_stmt = ast.Return(
-            value=ast.DictComp(
-                key=ast.Name(id="k"),
-                value=ast.Subscript(
-                    value=ast.Name(id="result"),
-                    slice=ast.Name(id="k"),
-                ),
-                generators=[
-                    ast.comprehension(
-                        target=ast.Name(id="k"), iter=output_list, ifs=[], is_async=0
-                    )
-                ],
-            )
+    new_class = tree.body[0]
+    # TODO add this manually
+    for stmt in new_class.body:
+        if isinstance(stmt, ast.FunctionDef) and stmt.name == "__init__":
+            stmt.name = "__user_init__"
+
+    # change the module that the code will reference
+    # this is required for the @serializable to mount it in the right path for serde
+    new_line = ast.parse('__module__ = "syft.user"')
+    new_class.body.append(new_line.body[0])
+    new_line = ast.parse(f'__canonical_name__ = "{class_name}"')
+    new_class.body.append(new_line.body[0])
+    new_line = ast.parse("__version__ = 1")
+    new_class.body.append(new_line.body[0])
+    new_class.name = class_name
+    new_class.decorator_list = [serializable_decorator]
+    new_body = []
+    new_body.append(
+        ast.ImportFrom(
+            module="__future__",
+            names=[ast.alias(name="annotations", asname="annotations")],
+            level=0,
         )
-        # requires typing module imported but main code returned is FunctionDef not Module
-        # return_annotation = ast.parse("typing.Dict[str, typing.Any]", mode="eval").body
-    else:
-        return_stmt = ast.Return(value=ast.Name(id="result"))
-        # requires typing module imported but main code returned is FunctionDef not Module
-        # return_annotation = ast.parse("typing.Any", mode="eval").body
-
-    new_body = tree.body + [call_stmt, return_stmt]
-
-    wrapper_function = ast.FunctionDef(
-        name=func_name,
-        args=f.args,
-        body=new_body,
-        decorator_list=[],
-        returns=None,
-        lineno=0,
     )
-
-    return astunparse.unparse(wrapper_function)
+    new_body.append(ast.Import(names=[ast.alias(name="syft", asname="sy")], level=0))
+    typing_types = [
+        "Any",
+        "Callable",
+        "ClassVar",
+        "Dict",
+        "List",
+        "Optional",
+        "Set",
+        "Tuple",
+        "Type",
+    ]
+    for typing_type in typing_types:
+        new_body.append(
+            ast.ImportFrom(
+                module="typing",
+                names=[ast.alias(name=typing_type, asname=typing_type)],
+                level=0,
+            )
+        )
+    new_body.append(new_class)
+    module = ast.Module(new_body, type_ignores=[])
+    try:
+        return unparse(module)
+    except Exception as e:
+        print("failed to unparse", e)
+        raise e
 
 
-def new_check_code(context: TransformContext) -> TransformContext:
+def check_class_code(context: TransformContext) -> TransformContext:
+    # TODO: define the proper checking for this case based on the ideas from UserCode
+    # check for no globals
+    # check for Policy template -> __init__, apply_output, public_state
+    # parse init signature
+    # check dangerous libraries, maybe compile_restricted already does that
     try:
-        processed_code = process_code(
+        processed_code = process_class_code(
             raw_code=context.output["raw_code"],
-            func_name=context.output["unique_func_name"],
-            original_func_name=context.output["service_func_name"],
-            input_policy=context.output["input_policy"],
-            output_policy=context.output["output_policy"],
+            class_name=context.output["unique_name"],
         )
         context.output["parsed_code"] = processed_code
-
     except Exception as e:
         raise e
-
     return context
 
 
-def compile_byte_code(parsed_code: str) -> Optional[PyCodeObject]:
-    try:
-        return compile(parsed_code, "<string>", "exec")
-    except Exception as e:
-        print("WARNING: to compile byte code", e)
-    return None
-
-
 def compile_code(context: TransformContext) -> TransformContext:
     byte_code = compile_byte_code(context.output["parsed_code"])
     if byte_code is None:
         raise Exception(
             "Unable to compile byte code from parsed code. "
             + context.output["parsed_code"]
         )
     return context
 
 
-def hash_code(context: TransformContext) -> TransformContext:
-    code = context.output["code"]
-    del context.output["code"]
-    context.output["raw_code"] = code
-    code_hash = hashlib.sha256(code.encode("utf8")).hexdigest()
-    context.output["code_hash"] = code_hash
-    return context
-
-
 def add_credentials_for_key(key: str) -> Callable:
     def add_credentials(context: TransformContext) -> TransformContext:
         context.output[key] = context.credentials
         return context
 
     return add_credentials
 
 
 def generate_signature(context: TransformContext) -> TransformContext:
     params = [
         Parameter(name=k, kind=Parameter.POSITIONAL_OR_KEYWORD)
-        for k in context.output["input_policy"].inputs.keys()
+        for k in context.output["input_kwargs"]
     ]
     sig = Signature(parameters=params)
     context.output["signature"] = sig
     return context
 
 
-def modify_signature(context: TransformContext) -> TransformContext:
-    sig = context.output["signature"]
-    context.output["signature"] = sig.replace(return_annotation=Dict[str, Any])
-    return context
-
-
-def check_input_policy(context: TransformContext) -> TransformContext:
-    ip = context.output["input_policy"]
-    ip.node_uid = context.node.id
-    context.output["input_policy"] = ip
-    return context
-
-
-def init_output_policy_state(context: TransformContext) -> TransformContext:
-    context.output["output_policy_state"] = context.output["output_policy"].state_type()
-    return context
-
-
-def add_custom_status(context: TransformContext) -> TransformContext:
-    if context.node.node_type == NodeType.DOMAIN:
-        node_view = NodeView(
-            node_name=context.node.name, verify_key=context.node.signing_key.verify_key
-        )
-        if node_view in context.obj.input_policy.inputs.keys():
-            context.output["status"] = UserCodeStatusContext(
-                base_dict={node_view: UserCodeStatus.SUBMITTED}
-            )
-        else:
-            raise NotImplementedError
-    elif context.node.node_type == NodeType.ENCLAVE:
-        base_dict = {
-            key: UserCodeStatus.SUBMITTED
-            for key in context.obj.input_policy.inputs.keys()
-        }
-
-        context.output["status"] = UserCodeStatusContext(base_dict=base_dict)
-    else:
-        # Consult with Madhava, on propogating errors from transforms
-        raise NotImplementedError
-    return context
-
-
-@transform(SubmitUserCode, UserCode)
-def submit_user_code_to_user_code() -> List[Callable]:
+@transform(SubmitUserPolicy, UserPolicy)
+def submit_policy_code_to_user_code() -> List[Callable]:
     return [
         generate_id,
         hash_code,
-        generate_unique_func_name,
-        modify_signature,
-        new_check_code,
-        # compile_code, # don't compile code till its approved
+        generate_unique_class_name,
+        generate_signature,
+        check_class_code,
+        # compile_code, # don't compile until approved
         add_credentials_for_key("user_verify_key"),
-        check_input_policy,
-        init_output_policy_state,
-        add_custom_status,
     ]
 
 
-@serializable()
-class UserCodeExecutionResult(SyftObject):
-    # version
-    __canonical_name__ = "UserCodeExecutionResult"
-    __version__ = SYFT_OBJECT_VERSION_1
-
-    id: UID
-    user_code_id: UID
-    stdout: str
-    stderr: str
-    result: Any
+def add_class_to_user_module(klass: type, unique_name: str) -> type:
+    klass.__module__ = "syft.user"
+    klass.__name__ = unique_name
+    # syft absolute
+    import syft as sy
+
+    if not hasattr(sy, "user"):
+        user_module = types.ModuleType("user")
+        setattr(sys.modules["syft"], "user", user_module)
+    user_module = sy.user
+    setattr(user_module, unique_name, klass)
+    setattr(sys.modules["syft"], "user", user_module)
+    return klass
 
 
-def execute_byte_code(code_item: UserCode, kwargs: Dict[str, Any]) -> Any:
+def execute_policy_code(user_policy: UserPolicy):
     stdout_ = sys.stdout
     stderr_ = sys.stderr
 
     try:
         stdout = StringIO()
         stderr = StringIO()
 
         sys.stdout = stdout
         sys.stderr = stderr
 
-        # statisfy lint checker
-        result = None
-
-        exec(code_item.byte_code)  # nosec
+        class_name = f"{user_policy.unique_name}"
+        if class_name in user_policy.__object_version_registry__.keys():
+            policy_class = user_policy.__object_version_registry__[class_name]
+        else:
+            exec(user_policy.byte_code)  # nosec
+            policy_class = eval(user_policy.unique_name)  # nosec
 
-        evil_string = f"{code_item.unique_func_name}(**kwargs)"
-        result = eval(evil_string, None, locals())  # nosec
+        policy_class = add_class_to_user_module(policy_class, user_policy.unique_name)
 
-        # restore stdout and stderr
         sys.stdout = stdout_
         sys.stderr = stderr_
 
-        return UserCodeExecutionResult(
-            user_code_id=code_item.id,
-            stdout=str(stdout.getvalue()),
-            stderr=str(stderr.getvalue()),
-            result=result,
-        )
+        return policy_class
 
     except Exception as e:
         print("execute_byte_code failed", e, file=stderr_)
+
     finally:
         sys.stdout = stdout_
         sys.stderr = stderr_
+
+
+def load_policy_code(user_policy: UserPolicy) -> Any:
+    try:
+        policy_class = execute_policy_code(user_policy)
+        return policy_class
+    except Exception as e:
+        raise Exception(f"Exception loading code. {user_policy}. {e}")
+
+
+def init_policy(user_policy: UserPolicy, init_args: Dict[str, Any]):
+    policy_class = load_policy_code(user_policy)
+    policy_object = policy_class()
+    policy_object.__user_init__(**init_args)
+    return policy_object
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/user_code_parse.py` & `syft-0.8.0b7/src/syft/core/node/new/user_code_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # stdlib
 import ast
 from typing import List
 
-# third party
-import astunparse  # ast.unparse for python 3.8
+# relative
+from .unparse import unparse
 
 
 class GlobalsVisitor(ast.NodeVisitor):
     def generic_visit(self, node):
         if isinstance(node, ast.Global):
             raise Exception("No Globals allows")
         ast.NodeVisitor.generic_visit(self, node)
@@ -64,8 +64,8 @@
     wrapper_function = make_ast_func(
         func_name,
         input_kwargs=input_kwargs,
         output_arg=output_arg,
         body=ast_code.body,
     )
 
-    return astunparse.unparse(wrapper_function)
+    return unparse(wrapper_function)
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/user_code_service.py` & `syft-0.8.0b7/src/syft/core/node/new/user_code_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,25 +8,30 @@
 from result import OkErr
 
 # relative
 from ....telemetry import instrument
 from .context import AuthedServiceContext
 from .document_store import DocumentStore
 from .linked_obj import LinkedObject
+from .policy import OutputHistory
+from .policy import UserPolicy
+from .policy import load_policy_code
+from .request import SubmitRequest
 from .request import UserCodeStatusChange
+from .request_service import RequestService
 from .response import SyftError
 from .response import SyftNotReady
 from .response import SyftSuccess
 from .serializable import serializable
 from .service import AbstractService
 from .service import SERVICE_TO_TYPES
 from .service import TYPE_TO_SERVICE
 from .service import service_method
+from .twin_object import TwinObject
 from .uid import UID
-from .user_code import OutputHistory
 from .user_code import SubmitUserCode
 from .user_code import UserCode
 from .user_code import UserCodeStatus
 from .user_code_stash import UserCodeStash
 from .user_roles import GUEST_ROLE_LEVEL
 
 
@@ -41,39 +46,38 @@
         self.stash = UserCodeStash(store=store)
 
     @service_method(path="code.submit", name="submit")
     def submit(
         self, context: AuthedServiceContext, code: SubmitUserCode
     ) -> Union[UserCode, SyftError]:
         """Add User Code"""
-        result = self.stash.set(code.to(UserCode, context=context))
+        user_code = code.to(UserCode, context=context)
+        result = self.stash.set(user_code)
         if result.is_err():
             return SyftError(message=str(result.err()))
         return SyftSuccess(message="User Code Submitted")
 
     def _code_execution(
         self,
         context: AuthedServiceContext,
         code: SubmitUserCode,
     ):
-        # relative
-        from .request import SubmitRequest
-        from .request_service import RequestService
-
         user_code = code.to(UserCode, context=context)
         result = self.stash.set(user_code)
         if result.is_err():
             return SyftError(message=str(result.err()))
 
         linked_obj = LinkedObject.from_obj(user_code, node_uid=context.node.id)
 
         CODE_EXECUTE = UserCodeStatusChange(
             value=UserCodeStatus.EXECUTE, linked_obj=linked_obj
         )
-        request = SubmitRequest(changes=[CODE_EXECUTE])
+        changes = [CODE_EXECUTE]
+
+        request = SubmitRequest(changes=changes)
         method = context.node.get_service_method(RequestService.submit)
         result = method(context=context, request=request)
 
         # The Request service already returns either a SyftSuccess or SyftError
         return result
 
     @service_method(
@@ -100,15 +104,19 @@
     @service_method(path="code.get_by_id", name="get_by_id")
     def get_by_uid(
         self, context: AuthedServiceContext, uid: UID
     ) -> Union[SyftSuccess, SyftError]:
         """Get a User Code Item"""
         result = self.stash.get_by_uid(uid=uid)
         if result.is_ok():
-            return result.ok()
+            user_code = result.ok()
+            if user_code.input_policy_state:
+                # TODO replace with LinkedObject Context
+                user_code.node_uid = context.node.id
+            return user_code
         return SyftError(message=result.err())
 
     @service_method(path="code.get_all_for_user", name="get_all_for_user")
     def get_all_for_user(
         self, context: AuthedServiceContext
     ) -> Union[SyftSuccess, SyftError]:
         """Get All User Code Items for User's VerifyKey"""
@@ -122,70 +130,83 @@
         self, context: AuthedServiceContext, code_item: UserCode
     ) -> Union[SyftSuccess, SyftError]:
         result = self.stash.update(code_item)
         if result.is_ok():
             return SyftSuccess(message="Code State Updated")
         return SyftError(message="Unable to Update Code State")
 
+    def load_user_code(self) -> None:
+        result = self.stash.get_all()
+        if result.is_ok():
+            user_code_items = result.ok()
+            for user_code in user_code_items:
+                if user_code.status.approved:
+                    if isinstance(user_code.input_policy_type, UserPolicy):
+                        load_policy_code(user_code.input_policy_type)
+                    if isinstance(user_code.output_policy_type, UserPolicy):
+                        load_policy_code(user_code.output_policy_type)
+
     @service_method(path="code.call", name="call", roles=GUEST_ROLE_LEVEL)
     def call(
         self, context: AuthedServiceContext, uid: UID, **kwargs: Any
     ) -> Union[SyftSuccess, SyftError]:
         """Call a User Code Function"""
         try:
             filtered_kwargs = filter_kwargs(kwargs)
             result = self.stash.get_by_uid(uid=uid)
-            if result.is_ok():
-                code_item = result.ok()
-                if code_item.status.for_context(context) == UserCodeStatus.EXECUTE:
-                    is_valid = code_item.output_policy_state.valid
-                    if not is_valid:
-                        if (
-                            len(
-                                code_item.output_policy_state.output_history,
-                            )
-                            > 0
-                        ):
-                            return get_outputs(
-                                context=context,
-                                output_history=code_item.output_policy_state.output_history[
-                                    -1
-                                ],
-                            )
-                        return is_valid
-                    else:
-                        action_service = context.node.get_service("actionservice")
-                        result = action_service._user_code_execute(
-                            context, code_item, filtered_kwargs
-                        )
-                        if isinstance(result, str):
-                            return SyftError(message=result)
-                        if result.is_ok():
-                            result = result.ok()
-                            code_item.output_policy_state.update_state(
-                                context=context, outputs=result.id
-                            )
-
-                            state_result = self.update_code_state(
-                                context=context, code_item=code_item
-                            )
-
-                            if state_result:
-                                return result
-                            else:
-                                return state_result
-                elif code_item.status.for_context(context) == UserCodeStatus.SUBMITTED:
+            if not result.is_ok():
+                return SyftError(message=result.err())
+
+            # Unroll variables
+            code_item = result.ok()
+            status = code_item.status
+
+            # Check if we are allowed to execute the code
+            if status.for_context(context) != UserCodeStatus.EXECUTE:
+                if status.for_context(context) == UserCodeStatus.SUBMITTED:
                     return SyftNotReady(
-                        message=f"{type(code_item)} Your code is waiting for approval: {code_item.status}"
+                        message=f"{type(code_item)} Your code is waiting for approval: {status}"
                     )
-                else:
-                    return SyftError(
-                        message=f"{type(code_item)} Your code cannot be run: {code_item.status}"
+                return SyftError(
+                    message=f"{type(code_item)} Your code cannot be run: {status}"
+                )
+
+            output_policy = code_item.output_policy
+            if output_policy is None:
+                raise Exception("Output policy not approved", code_item)
+
+            # Check if the OutputPolicy is valid
+            is_valid = output_policy.valid
+
+            if not is_valid:
+                if len(output_policy.output_history) > 0:
+                    return get_outputs(
+                        context=context,
+                        output_history=output_policy.output_history[-1],
                     )
-            return SyftError(message=result.err())
+                return is_valid
+
+            # Execute the code item
+            action_service = context.node.get_service("actionservice")
+            result = action_service._user_code_execute(
+                context, code_item, filtered_kwargs
+            )
+            if isinstance(result, str):
+                return SyftError(message=result)
+
+            # Apply Output Policy to the results and update the OutputPolicyState
+            final_results = result.ok()
+            output_policy.apply_output(context=context, outputs=final_results)
+            code_item.output_policy = output_policy
+            state_result = self.update_code_state(context=context, code_item=code_item)
+            if not state_result:
+                return state_result
+            if isinstance(final_results, TwinObject):
+                return final_results.private
+            return final_results
         except Exception as e:
             return SyftError(message=f"Failed to run. {e}")
 
 
 def get_outputs(context: AuthedServiceContext, output_history: OutputHistory) -> Any:
     # relative
     from .action_service import TwinMode
```

### Comparing `syft-0.8.0b6/src/syft/core/node/new/user_code_stash.py` & `syft-0.8.0b7/src/syft/core/node/new/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/user_roles.py` & `syft-0.8.0b7/src/syft/core/node/new/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/user_service.py` & `syft-0.8.0b7/src/syft/core/node/new/user_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/user_stash.py` & `syft-0.8.0b7/src/syft/core/node/new/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/util.py` & `syft-0.8.0b7/src/syft/core/node/new/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/verification.py` & `syft-0.8.0b7/src/syft/core/node/new/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/new/worker_settings.py` & `syft-0.8.0b7/src/syft/core/node/new/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/core/node/worker.py` & `syft-0.8.0b7/src/syft/core/node/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 
 # stdlib
 import contextlib
 from datetime import datetime
 from functools import partial
 import hashlib
 import os
+import threading
 from typing import Any
 from typing import Callable
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
 
 # third party
 import gevent
@@ -50,14 +52,15 @@
 from .new.message_service import MessageService
 from .new.metadata_service import MetadataService
 from .new.metadata_stash import MetadataStash
 from .new.network_service import NetworkService
 from .new.node import NewNode
 from .new.node import NodeType
 from .new.node_metadata import NodeMetadata
+from .new.policy_service import PolicyService
 from .new.project_service import ProjectService
 from .new.queue_stash import QueueItem
 from .new.queue_stash import QueueStash
 from .new.request_service import RequestService
 from .new.response import SyftError
 from .new.serializable import serializable
 from .new.serialize import _serialize
@@ -76,14 +79,23 @@
 from .new.user_code_service import UserCodeService
 from .new.user_roles import ServiceRole
 from .new.user_service import UserService
 from .new.user_stash import UserStash
 from .new.worker_settings import WorkerSettings
 
 
+def thread_ident() -> int:
+    return threading.current_thread().ident
+
+
+# if user code needs to be serded and its not available we can call this to refresh
+# the code for a specific node UID and thread
+CODE_RELOADER: Dict[int, Callable] = {}
+
+
 def gipc_encoder(obj):
     return _serialize(obj, to_bytes=True)
 
 
 def gipc_decoder(obj_bytes):
     return _deserialize(obj_bytes, from_bytes=True)
 
@@ -163,14 +175,15 @@
                 ActionService,
                 TestService,
                 DatasetService,
                 UserCodeService,
                 RequestService,
                 DataSubjectService,
                 NetworkService,
+                PolicyService,
                 MessageService,
                 ProjectService,
                 DataSubjectMemberService,
             ]
             if services is None
             else services
         )
@@ -216,15 +229,31 @@
     ) -> Self:
         name_hash = hashlib.sha256(name.encode("utf8")).digest()
         uid = UID(name_hash[0:16])
         key = SyftSigningKey(SigningKey(name_hash))
         if reset:
             store_config = SQLiteStoreClientConfig()
             store_config.filename = f"{uid}.sqlite"
-            with contextlib.suppress(FileNotFoundError):
+
+            # stdlib
+            import sqlite3
+
+            with contextlib.closing(sqlite3.connect(store_config.file_path)) as db:
+                cursor = db.cursor()
+                cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
+                tables = cursor.fetchall()
+
+                for table_name in tables:
+                    drop_table_sql = f"DROP TABLE IF EXISTS {table_name[0]};"
+                    cursor.execute(drop_table_sql)
+
+                db.commit()
+                db.close()
+
+            with contextlib.suppress(FileNotFoundError, PermissionError):
                 if os.path.exists(store_config.file_path):
                     os.unlink(store_config.file_path)
 
         return cls(
             name=name,
             id=uid,
             signing_key=key,
@@ -254,19 +283,23 @@
         connection = PythonConnection(node=self)
         return SyftClient(connection=connection, credentials=SyftSigningKey.generate())
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}: {self.name} - {self.id} - {self.node_type} - {self.services}"
 
     def post_init(self) -> None:
+        if UserCodeService in self.services:
+            user_code_service = self.get_service(UserCodeService)
+            user_code_service.load_user_code()
         if self.is_subprocess:
             # print(f"> Starting Subprocess {self}")
             pass
         else:
             print(f"> Starting {self}")
+        CODE_RELOADER[thread_ident()] = user_code_service.load_user_code
         # super().post_init()
 
     def init_stores(
         self,
         document_store_config: Optional[StoreConfig] = None,
         action_store_config: Optional[StoreConfig] = None,
     ):
@@ -325,14 +358,15 @@
                 UserService,
                 MetadataService,
                 DatasetService,
                 UserCodeService,
                 RequestService,
                 DataSubjectService,
                 NetworkService,
+                PolicyService,
                 MessageService,
                 ProjectService,
                 DataSubjectMemberService,
             ]
 
             if OBLV:
                 # relative
```

### Comparing `syft-0.8.0b6/src/syft/deploy.py` & `syft-0.8.0b7/src/syft/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/experimental_flags.py` & `syft-0.8.0b7/src/syft/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/external/__init__.py` & `syft-0.8.0b7/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/external/oblv/__init__.py` & `syft-0.8.0b7/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/external/oblv/deployment.py` & `syft-0.8.0b7/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/external/oblv/deployment_client.py` & `syft-0.8.0b7/src/syft/external/oblv/deployment_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/external/oblv/exceptions.py` & `syft-0.8.0b7/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/external/oblv/oblv_keys.py` & `syft-0.8.0b7/src/syft/external/oblv/oblv_keys.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.0b7/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.0b7/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/external/oblv/oblv_service.py` & `syft-0.8.0b7/src/syft/external/oblv/oblv_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/filterwarnings.py` & `syft-0.8.0b7/src/syft/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/gevent_patch.py` & `syft-0.8.0b7/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/logger.py` & `syft-0.8.0b7/src/syft/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/registry.py` & `syft-0.8.0b7/src/syft/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/search.py` & `syft-0.8.0b7/src/syft/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/telemetry.py` & `syft-0.8.0b7/src/syft/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/trace_decorator.py` & `syft-0.8.0b7/src/syft/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/user_settings.py` & `syft-0.8.0b7/src/syft/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft/util.py` & `syft-0.8.0b7/src/syft/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,21 +135,15 @@
     if fully_qualified_name == "builtins.NoneType":
         fully_qualified_name = "syft.lib.python._SyNone"
     attr_list = fully_qualified_name.split(".")
 
     if attr_list[0] != "syft":
         raise ReferenceError(f"Reference don't match: {attr_list[0]}")
 
-    if (
-        attr_list[1] != "core"
-        and attr_list[1] != "lib"
-        and attr_list[1] != "grid"
-        and attr_list[1] != "wrappers"
-        and attr_list[1] != "proxy"
-    ):
+    if attr_list[1] != "core" and attr_list[1] != "user":
         raise ReferenceError(f"Reference don't match: {attr_list[1]}")
 
     return index_modules(a_dict=get_loaded_syft(), keys=attr_list[1:])
 
 
 def get_fully_qualified_name(obj: object) -> str:
     """Return the full path and name of a class
@@ -726,7 +720,28 @@
         # set start method to fork in case of MacOS
         set_start_method("fork", force=True)
 
     multiprocessing.Process(
         target=print_process, args=(message, finish, success, lock)
     ).start()
     return (finish, success)
+
+
+# Note: In the future there might be other interpreters that we want to use
+def is_interpreter_jupyter() -> bool:
+    return get_interpreter_module() == "ipykernel.zmqshell"
+
+
+def is_interpreter_colab() -> bool:
+    return get_interpreter_module() == "google.colab._shell"
+
+
+def is_interpreter_standard() -> bool:
+    return get_interpreter_module() == "StandardInterpreter"
+
+
+def get_interpreter_module() -> str:
+    try:
+        shell = get_ipython().__class__.__module__
+        return shell
+    except NameError:
+        return "StandardInterpreter"  # not sure
```

### Comparing `syft-0.8.0b6/src/syft/version_compare.py` & `syft-0.8.0b7/src/syft/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b6/src/syft.egg-info/PKG-INFO` & `syft-0.8.0b7/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.0b6
+Version: 0.8.0b7
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.0b6 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.0b7 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.8 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.0b6/src/syft.egg-info/SOURCES.txt` & `syft-0.8.0b7/src/syft.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 src/syft/core/node/new/action_types.py
 src/syft/core/node/new/api.py
 src/syft/core/node/new/array.py
 src/syft/core/node/new/arrow.py
 src/syft/core/node/new/base.py
 src/syft/core/node/new/capnp.py
 src/syft/core/node/new/client.py
+src/syft/core/node/new/code_parse.py
 src/syft/core/node/new/connection.py
 src/syft/core/node/new/context.py
 src/syft/core/node/new/credentials.py
 src/syft/core/node/new/data_subject.py
 src/syft/core/node/new/data_subject_member.py
 src/syft/core/node/new/data_subject_member_service.py
 src/syft/core/node/new/data_subject_service.py
@@ -72,14 +73,16 @@
 src/syft/core/node/new/mongo_codecs.py
 src/syft/core/node/new/mongo_document_store.py
 src/syft/core/node/new/network_service.py
 src/syft/core/node/new/node.py
 src/syft/core/node/new/node_metadata.py
 src/syft/core/node/new/numpy.py
 src/syft/core/node/new/pandas.py
+src/syft/core/node/new/policy.py
+src/syft/core/node/new/policy_service.py
 src/syft/core/node/new/project.py
 src/syft/core/node/new/project_service.py
 src/syft/core/node/new/project_stash.py
 src/syft/core/node/new/queue_stash.py
 src/syft/core/node/new/recursive.py
 src/syft/core/node/new/recursive_primitives.py
 src/syft/core/node/new/request.py
@@ -94,19 +97,21 @@
 src/syft/core/node/new/sqlite_document_store.py
 src/syft/core/node/new/syft_object.py
 src/syft/core/node/new/test_service.py
 src/syft/core/node/new/third_party.py
 src/syft/core/node/new/transforms.py
 src/syft/core/node/new/twin_object.py
 src/syft/core/node/new/uid.py
+src/syft/core/node/new/unparse.py
 src/syft/core/node/new/user.py
 src/syft/core/node/new/user_code.py
 src/syft/core/node/new/user_code_parse.py
 src/syft/core/node/new/user_code_service.py
 src/syft/core/node/new/user_code_stash.py
+src/syft/core/node/new/user_policy_stash.py
 src/syft/core/node/new/user_roles.py
 src/syft/core/node/new/user_service.py
 src/syft/core/node/new/user_stash.py
 src/syft/core/node/new/util.py
 src/syft/core/node/new/verification.py
 src/syft/core/node/new/worker_settings.py
 src/syft/external/__init__.py
```

### Comparing `syft-0.8.0b6/src/syft.egg-info/requires.txt` & `syft-0.8.0b7/src/syft.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 pytest-parallel
 pytest-asyncio
 pytest-randomly
 pytest-sugar
 pytest_mock_resources
 python_on_whales
 pytest-lazy-fixture
+pytest-rerunfailures
 coverage
 joblib
 faker
 bandit==1.7.5
 ruff==0.0.254
 importlib-metadata==6.0.0
 isort==5.12.0
@@ -62,10 +63,11 @@
 pytest-parallel
 pytest-asyncio
 pytest-randomly
 pytest-sugar
 pytest_mock_resources
 python_on_whales
 pytest-lazy-fixture
+pytest-rerunfailures
 coverage
 joblib
 faker
```

