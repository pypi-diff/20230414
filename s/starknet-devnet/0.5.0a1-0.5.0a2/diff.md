# Comparing `tmp/starknet_devnet-0.5.0a1.tar.gz` & `tmp/starknet_devnet-0.5.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starknet_devnet-0.5.0a1.tar", max compression
+gzip compressed data, was "starknet_devnet-0.5.0a2.tar", max compression
```

## Comparing `starknet_devnet-0.5.0a1.tar` & `starknet_devnet-0.5.0a2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1046 2023-03-29 08:54:42.832564 starknet_devnet-0.5.0a1/README.md
--rw-r--r--   0        0        0     1796 2023-03-29 08:54:42.840564 starknet_devnet-0.5.0a1/pyproject.toml
--rw-r--r--   0        0        0   208485 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json
--rw-r--r--   0        0        0    32743 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/MockStarknetMessaging.json
--rw-r--r--   0        0        0    35645 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/UDC_OZ_0.5.0.json
--rw-r--r--   0        0        0     2563 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/__init__.py
--rw-r--r--   0        0        0     2130 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/account.py
--rw-r--r--   0        0        0     3784 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/account_util.py
--rw-r--r--   0        0        0     2692 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/accounts.py
--rw-r--r--   0        0        0   118818 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json
--rw-r--r--   0        0        0     1784 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json
--rw-r--r--   0        0        0     1866 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/block_info_generator.py
--rw-r--r--   0        0        0    11423 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/blocks.py
--rw-r--r--   0        0        0        0 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/__init__.py
--rw-r--r--   0        0        0     7067 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/base.py
--rw-r--r--   0        0        0    13712 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/feeder_gateway.py
--rw-r--r--   0        0        0     2167 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/gateway.py
--rw-r--r--   0        0        0     3959 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/postman.py
--rw-r--r--   0        0        0        0 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/__init__.py
--rw-r--r--   0        0        0     2120 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/blocks.py
--rw-r--r--   0        0        0     2136 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/call.py
--rw-r--r--   0        0        0     2375 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/classes.py
--rw-r--r--   0        0        0     5341 2023-03-29 08:54:42.844564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/misc.py
--rw-r--r--   0        0        0     4958 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/routes.py
--rw-r--r--   0        0        0    79264 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/rpc_spec.py
--rw-r--r--   0        0        0     7466 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/rpc_spec_write.py
--rw-r--r--   0        0        0     7264 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/schema.py
--rw-r--r--   0        0        0     1144 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/state.py
--rw-r--r--   0        0        0      929 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/storage.py
--rw-r--r--   0        0        0        0 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/structures/__init__.py
--rw-r--r--   0        0        0    23046 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/structures/payloads.py
--rw-r--r--   0        0        0     6528 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/structures/responses.py
--rw-r--r--   0        0        0     3075 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/structures/types.py
--rw-r--r--   0        0        0     7298 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/transactions.py
--rw-r--r--   0        0        0     3328 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/utils.py
--rw-r--r--   0        0        0      899 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/blueprints/shared.py
--rw-r--r--   0        0        0    17030 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/cairo_rs_py_patch.py
--rw-r--r--   0        0        0      877 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/chargeable_account.py
--rw-r--r--   0        0        0     2851 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/compiler.py
--rw-r--r--   0        0        0      924 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/constants.py
--rw-r--r--   0        0        0      646 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/contract_class_wrapper.py
--rw-r--r--   0        0        0    13697 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/devnet_config.py
--rw-r--r--   0        0        0      784 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/dump.py
--rw-r--r--   0        0        0     5592 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/fee_token.py
--rw-r--r--   0        0        0     6872 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/forked_state.py
--rw-r--r--   0        0        0     1732 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/general_config.py
--rw-r--r--   0        0        0     8643 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/origin.py
--rw-r--r--   0        0        0     9901 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/postman_wrapper.py
--rw-r--r--   0        0        0     2005 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/predeployed_contract_wrapper.py
--rw-r--r--   0        0        0     4275 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/server.py
--rw-r--r--   0        0        0    38350 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/starknet_wrapper.py
--rw-r--r--   0        0        0     1988 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/state.py
--rw-r--r--   0        0        0     2113 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/state_archive.py
--rw-r--r--   0        0        0    11125 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/transactions.py
--rw-r--r--   0        0        0     1626 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/udc.py
--rw-r--r--   0        0        0     7968 2023-03-29 08:54:42.848564 starknet_devnet-0.5.0a1/starknet_devnet/util.py
--rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 starknet_devnet-0.5.0a1/setup.py
--rw-r--r--   0        0        0     2124 1970-01-01 00:00:00.000000 starknet_devnet-0.5.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1046 2023-04-05 11:29:38.195896 starknet_devnet-0.5.0a2/README.md
+-rw-r--r--   0        0        0     1795 2023-04-05 11:29:38.207896 starknet_devnet-0.5.0a2/pyproject.toml
+-rw-r--r--   0        0        0   208485 2023-04-05 11:29:38.207896 starknet_devnet-0.5.0a2/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json
+-rw-r--r--   0        0        0    32743 2023-04-05 11:29:38.207896 starknet_devnet-0.5.0a2/starknet_devnet/MockStarknetMessaging.json
+-rw-r--r--   0        0        0    35645 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/UDC_OZ_0.5.0.json
+-rw-r--r--   0        0        0     2563 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/__init__.py
+-rw-r--r--   0        0        0     2130 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/account.py
+-rw-r--r--   0        0        0     3784 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/account_util.py
+-rw-r--r--   0        0        0     2692 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/accounts.py
+-rw-r--r--   0        0        0   118818 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json
+-rw-r--r--   0        0        0     1784 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json
+-rw-r--r--   0        0        0     1866 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/block_info_generator.py
+-rw-r--r--   0        0        0    11423 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blocks.py
+-rw-r--r--   0        0        0        0 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/__init__.py
+-rw-r--r--   0        0        0     7067 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/base.py
+-rw-r--r--   0        0        0    13712 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/feeder_gateway.py
+-rw-r--r--   0        0        0     2167 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/gateway.py
+-rw-r--r--   0        0        0     3959 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/postman.py
+-rw-r--r--   0        0        0        0 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/__init__.py
+-rw-r--r--   0        0        0     2120 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/blocks.py
+-rw-r--r--   0        0        0     2136 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/call.py
+-rw-r--r--   0        0        0     2375 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/classes.py
+-rw-r--r--   0        0        0     5341 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/misc.py
+-rw-r--r--   0        0        0     4958 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/routes.py
+-rw-r--r--   0        0        0    79264 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/rpc_spec.py
+-rw-r--r--   0        0        0     7466 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/rpc_spec_write.py
+-rw-r--r--   0        0        0     7264 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/schema.py
+-rw-r--r--   0        0        0     1144 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/state.py
+-rw-r--r--   0        0        0      929 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/storage.py
+-rw-r--r--   0        0        0        0 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/structures/__init__.py
+-rw-r--r--   0        0        0    23046 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/structures/payloads.py
+-rw-r--r--   0        0        0     6528 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/structures/responses.py
+-rw-r--r--   0        0        0     3075 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/structures/types.py
+-rw-r--r--   0        0        0     7298 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/transactions.py
+-rw-r--r--   0        0        0     3328 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/utils.py
+-rw-r--r--   0        0        0      899 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/shared.py
+-rw-r--r--   0        0        0    17030 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/cairo_rs_py_patch.py
+-rw-r--r--   0        0        0      877 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/chargeable_account.py
+-rw-r--r--   0        0        0     2851 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/compiler.py
+-rw-r--r--   0        0        0     1134 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/constants.py
+-rw-r--r--   0        0        0      646 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/contract_class_wrapper.py
+-rw-r--r--   0        0        0    13802 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/devnet_config.py
+-rw-r--r--   0        0        0      784 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/dump.py
+-rw-r--r--   0        0        0     5592 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/fee_token.py
+-rw-r--r--   0        0        0     6872 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/forked_state.py
+-rw-r--r--   0        0        0     1732 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/general_config.py
+-rw-r--r--   0        0        0     8643 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/origin.py
+-rw-r--r--   0        0        0    10193 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/postman_wrapper.py
+-rw-r--r--   0        0        0     2005 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/predeployed_contract_wrapper.py
+-rw-r--r--   0        0        0     4275 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/server.py
+-rw-r--r--   0        0        0    38350 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/starknet_wrapper.py
+-rw-r--r--   0        0        0     1988 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/state.py
+-rw-r--r--   0        0        0     2113 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/state_archive.py
+-rw-r--r--   0        0        0    11173 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/transactions.py
+-rw-r--r--   0        0        0     1626 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/udc.py
+-rw-r--r--   0        0        0     7968 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/util.py
+-rw-r--r--   0        0        0     2399 1970-01-01 00:00:00.000000 starknet_devnet-0.5.0a2/setup.py
+-rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 starknet_devnet-0.5.0a2/PKG-INFO
```

### Comparing `starknet_devnet-0.5.0a1/README.md` & `starknet_devnet-0.5.0a2/README.md`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/pyproject.toml` & `starknet_devnet-0.5.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "starknet_devnet"
-version = "0.5.0a1"
+version = "0.5.0a2"
 description = "A local testnet for Starknet"
 authors = ["FabijanC <fabijan.corak@gmail.com>"]
 license = "ISC"
 
 readme = "README.md"
 repository = "https://github.com/Shard-Labs/starknet-devnet"
 homepage = "https://github.com/Shard-Labs/starknet-devnet"
 keywords = ["starknet", "cairo", "testnet", "local", "server"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.10"
 Flask = {extras = ["async"], version = "~2.0.3"}
 flask-cors = "~3.0.10"
-cairo-lang = "0.11.0.1"
+cairo-lang = "0.11.0.2"
 Werkzeug = "~2.0.3"
 cloudpickle = "~2.1.0"
 crypto-cpp-py = "~1.2.0"
 marshmallow = "~3.17.0"
 typing-extensions = "~4.3.0"
 gunicorn = "~20.1.0"
 marshmallow-dataclass = "~8.4"
 jsonschema = "~4.17.0"
-web3 = "~5.31.4"
+web3 = "~6.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "~2.12.2"
 psutil = "~5.9.1"
 pytest-xdist = "~2.5.0"
 pylint-quotes = "~0.2.3"
 black = "~22.6"
```

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json` & `starknet_devnet-0.5.0a2/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/MockStarknetMessaging.json` & `starknet_devnet-0.5.0a2/starknet_devnet/MockStarknetMessaging.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/UDC_OZ_0.5.0.json` & `starknet_devnet-0.5.0a2/starknet_devnet/UDC_OZ_0.5.0.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/__init__.py` & `starknet_devnet-0.5.0a2/starknet_devnet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # pylint: disable=unused-import
 # pylint: disable=import-outside-toplevel
 
 import os
 import sys
 
-__version__ = "0.5.0a1"
+__version__ = "0.5.0a2"
 
 
 def _patch_pedersen_hash():
     """
     This is a monkey-patch to improve the performance of the devnet
     We are using c++ code for calculating the pedersen hashes
     instead of python implementation from cairo-lang package
```

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/account.py` & `starknet_devnet-0.5.0a2/starknet_devnet/account.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/account_util.py` & `starknet_devnet-0.5.0a2/starknet_devnet/account_util.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/accounts.py` & `starknet_devnet-0.5.0a2/starknet_devnet/accounts.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json` & `starknet_devnet-0.5.0a2/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json` & `starknet_devnet-0.5.0a2/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/block_info_generator.py` & `starknet_devnet-0.5.0a2/starknet_devnet/block_info_generator.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blocks.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blocks.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/base.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/base.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/feeder_gateway.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/feeder_gateway.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/gateway.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/gateway.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/postman.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/postman.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/blocks.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/blocks.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/call.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/call.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/classes.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/classes.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/misc.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/misc.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/routes.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/routes.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/rpc_spec.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/rpc_spec.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/rpc_spec_write.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/rpc_spec_write.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/schema.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/schema.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/state.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/storage.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/storage.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/structures/payloads.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/structures/payloads.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/structures/responses.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/structures/responses.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/structures/types.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/structures/types.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/transactions.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/transactions.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/rpc/utils.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/blueprints/shared.py` & `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/shared.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/cairo_rs_py_patch.py` & `starknet_devnet-0.5.0a2/starknet_devnet/cairo_rs_py_patch.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/chargeable_account.py` & `starknet_devnet-0.5.0a2/starknet_devnet/chargeable_account.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/compiler.py` & `starknet_devnet-0.5.0a2/starknet_devnet/compiler.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/contract_class_wrapper.py` & `starknet_devnet-0.5.0a2/starknet_devnet/contract_class_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/devnet_config.py` & `starknet_devnet-0.5.0a2/starknet_devnet/devnet_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 NETWORK_TO_URL = {
     "alpha-goerli": "https://alpha4.starknet.io",
     "alpha-goerli2": "https://alpha4-2.starknet.io",
     "alpha-mainnet": "https://alpha-mainnet.starknet.io",
 }
 NETWORK_NAMES = ", ".join(NETWORK_TO_URL.keys())
 CHAIN_IDS = ", ".join([member.name for member in StarknetChainId])
+DEFAULT_CHAIN_ID = StarknetChainId.TESTNET
 
 
 def _fork_network(network_id: str):
     """
     Return the URL corresponding to the provided name.
     If it's not one of predefined names, assumes it is already a URL.
     """
@@ -352,21 +353,21 @@
         help="Specify the block number where the --fork-network is forked; defaults to latest",
     )
     parser.add_argument(
         "--fork-retries",
         type=int,
         default=1,
         action=PositiveAction,
-        help="Specify the number of retries of failed HTTP requests sent to the network before giving up, defaults to 1",
+        help="Specify the number of retries of failed HTTP requests sent to the network before giving up; defaults to 1",
     )
     parser.add_argument(
         "--chain-id",
         type=_chain_id,
-        default=StarknetChainId.TESTNET,
-        help=f"Specify the chain id as string: {{{CHAIN_IDS}}}",
+        default=DEFAULT_CHAIN_ID,
+        help=f"Specify the chain id as one of: {{{CHAIN_IDS}}}; defaults to {DEFAULT_CHAIN_ID.name} ({hex(DEFAULT_CHAIN_ID.value)})",
     )
     parser.add_argument(
         "--disable-rpc-request-validation",
         action="store_true",
         help="Disable requests schema validation for RPC endpoints",
     )
     parser.add_argument(
```

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/dump.py` & `starknet_devnet-0.5.0a2/starknet_devnet/dump.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/fee_token.py` & `starknet_devnet-0.5.0a2/starknet_devnet/fee_token.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/forked_state.py` & `starknet_devnet-0.5.0a2/starknet_devnet/forked_state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/general_config.py` & `starknet_devnet-0.5.0a2/starknet_devnet/general_config.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/origin.py` & `starknet_devnet-0.5.0a2/starknet_devnet/origin.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/postman_wrapper.py` & `starknet_devnet-0.5.0a2/starknet_devnet/postman_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 This module wraps the usage of Postman for L1 <> L2 interaction.
 """
 import json
 from abc import ABC, abstractmethod
 from typing import Tuple
 
 from starkware.eth.eth_test_utils import EthAccount, EthContract
+from starkware.eth.web3_wrapper import web3_contract_create_filter_fix
 from starkware.solidity.utils import load_nearby_contract
 from starkware.starknet.business_logic.transaction.objects import InternalL1Handler
 from starkware.starknet.definitions.error_codes import StarknetErrorCode
+from starkware.starknet.services.api.feeder_gateway.response_objects import (
+    LATEST_BLOCK_ID,
+)
 from starkware.starknet.testing.starknet import Starknet
 from web3 import HTTPProvider, Web3
 from web3.middleware import geth_poa_middleware
 
 from .constants import L1_MESSAGE_CANCELLATION_DELAY, TIMEOUT_FOR_WEB3_REQUESTS
 from .util import StarknetDevnetException, fixed_length_hex
 
@@ -104,15 +108,15 @@
 
         if self.__postman_wrapper is None:
             return {}
 
         postman = self.__postman_wrapper.postman
 
         l1_to_l2_messages = json.loads(
-            Web3.toJSON(
+            Web3.to_json(
                 self.__postman_wrapper.l1_to_l2_message_filter.get_new_entries()
             )
         )
         l2_to_l1_messages = state.l2_to_l1_messages_log[
             postman.n_consumed_l2_to_l1_messages :
         ]
 
@@ -157,32 +161,33 @@
     def load_mock_messaging_contract_in_l1(self, starknet, contract_address):
         if contract_address is None:
             self.mock_starknet_messaging_contract = self.eth_account.deploy(
                 load_nearby_contract("MockStarknetMessaging"),
                 L1_MESSAGE_CANCELLATION_DELAY,
             )
         else:
-            address = Web3.toChecksumAddress(contract_address)
+            address = Web3.to_checksum_address(contract_address)
             contract_json = load_nearby_contract("MockStarknetMessaging")
             abi = contract_json["abi"]
             w3_contract = self.web3.eth.contract(abi=abi, address=address)
             self.mock_starknet_messaging_contract = EthContract(
                 self.web3, address, w3_contract, abi, self.eth_account
             )
 
         self.postman = Postman(self.mock_starknet_messaging_contract, starknet)
-        self.l1_to_l2_message_filter = self.mock_starknet_messaging_contract.w3_contract.events.LogMessageToL2.createFilter(
-            fromBlock="latest"
+        events = self.mock_starknet_messaging_contract.w3_contract.events
+        self.l1_to_l2_message_filter = events.LogMessageToL2.create_filter(
+            fromBlock=LATEST_BLOCK_ID
         )
 
 
 class Postman:
     """
     Postman class copied from starknet code base.
-    https://github.com/starkware-libs/cairo-lang/blob/v0.10.1/src/starkware/starknet/testing/postman.py
+    https://github.com/starkware-libs/cairo-lang/blob/v0.11.0.2/src/starkware/starknet/testing/postman.py
 
     Modifications were made in _handle_l1_to_l2_messages function.
     """
 
     def __init__(
         self,
         mock_starknet_messaging_contract: EthContract,
@@ -190,16 +195,17 @@
     ):
         self.mock_starknet_messaging_contract = mock_starknet_messaging_contract
         self.starknet = starknet
         self.n_consumed_l2_to_l1_messages = 0
 
         # Create a filter to collect LogMessageToL2 events.
         w3_contract = self.mock_starknet_messaging_contract.w3_contract
-        self.message_to_l2_filter = w3_contract.events.LogMessageToL2.createFilter(
-            fromBlock="latest"
+        web3_contract_create_filter_fix(w3_contract.events.LogMessageToL2)
+        self.message_to_l2_filter = w3_contract.events.LogMessageToL2.create_filter(
+            fromBlock=LATEST_BLOCK_ID
         )
 
     async def _handle_l1_to_l2_messages(self):
         transactions_to_execute = []
         for event in self.message_to_l2_filter.get_new_entries():
             args = event.args
             transaction = InternalL1Handler.create(
```

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/predeployed_contract_wrapper.py` & `starknet_devnet-0.5.0a2/starknet_devnet/predeployed_contract_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/server.py` & `starknet_devnet-0.5.0a2/starknet_devnet/server.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/starknet_wrapper.py` & `starknet_devnet-0.5.0a2/starknet_devnet/starknet_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/state.py` & `starknet_devnet-0.5.0a2/starknet_devnet/state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/state_archive.py` & `starknet_devnet-0.5.0a2/starknet_devnet/state_archive.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/transactions.py` & `starknet_devnet-0.5.0a2/starknet_devnet/transactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,17 @@
 
         contract_address = self.execution_info.call_info.contract_address
 
         for l2_to_l1_message in self.execution_info.get_sorted_l2_to_l1_messages():
             l2_to_l1_messages.append(
                 L2ToL1Message(
                     from_address=contract_address,
-                    to_address=Web3.toChecksumAddress(hex(l2_to_l1_message.to_address)),
+                    to_address=Web3.to_checksum_address(
+                        hex(l2_to_l1_message.to_address)
+                    ),
                     payload=l2_to_l1_message.payload,
                 )
             )
 
         return l2_to_l1_messages
 
     def __get_block_hash(self) -> int:
```

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/udc.py` & `starknet_devnet-0.5.0a2/starknet_devnet/udc.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/starknet_devnet/util.py` & `starknet_devnet-0.5.0a2/starknet_devnet/util.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a1/setup.py` & `starknet_devnet-0.5.0a2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 package_data = \
 {'': ['*'],
  'starknet_devnet': ['accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/*']}
 
 install_requires = \
 ['Flask[async]>=2.0.3,<2.1.0',
  'Werkzeug>=2.0.3,<2.1.0',
- 'cairo-lang==0.11.0.1',
+ 'cairo-lang==0.11.0.2',
  'cloudpickle>=2.1.0,<2.2.0',
  'crypto-cpp-py>=1.2.0,<1.3.0',
  'flask-cors>=3.0.10,<3.1.0',
  'gunicorn>=20.1.0,<20.2.0',
  'jsonschema>=4.17.0,<4.18.0',
  'marshmallow-dataclass>=8.4,<8.5',
  'marshmallow>=3.17.0,<3.18.0',
  'typing-extensions>=4.3.0,<4.4.0',
- 'web3>=5.31.4,<5.32.0']
+ 'web3>=6.0.0,<6.1.0']
 
 entry_points = \
 {'console_scripts': ['starknet-devnet = starknet_devnet.server:main']}
 
 setup_kwargs = {
     'name': 'starknet-devnet',
-    'version': '0.5.0a1',
+    'version': '0.5.0a2',
     'description': 'A local testnet for Starknet',
     'long_description': '<!-- logo / title -->\n<p align="center" style="margin-bottom: 0px !important">\n  <img width="200" src="https://user-images.githubusercontent.com/2848732/193076972-da6fa36e-11f7-4cb3-aa29-673224f8576d.png" alt="Devnet" align="center">\n</p>\n<h1 align="center" style="margin-top: 0px !important">Starknet Devnet</h1>\n\nA Flask wrapper of Starknet state. Similar in purpose to Ganache.\n\nAims to mimic Starknet\'s Alpha testnet, but with simplified functionality.\n\n## 🌐 Docs\n\nOn the following links you can find the documentation of:\n\n- [the latest official release](https://shard-labs.github.io/starknet-devnet/)\n- [the latest master commit (not officially released)](https://github.com/Shard-Labs/starknet-devnet/tree/master/page/docs)\n\n## ✏️ Contributing\n\nWe ❤️ and encourage all contributions!\n\n[Click here](https://shard-labs.github.io/starknet-devnet/docs/guide/development) for the development guide.\n\n## 🙌 Special Thanks\n\nSpecial thanks to all the [contributors](https://github.com/Shard-Labs/starknet-devnet/graphs/contributors)!\n',
     'author': 'FabijanC',
     'author_email': 'fabijan.corak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Shard-Labs/starknet-devnet',
```

### Comparing `starknet_devnet-0.5.0a1/PKG-INFO` & `starknet_devnet-0.5.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: starknet-devnet
-Version: 0.5.0a1
+Version: 0.5.0a2
 Summary: A local testnet for Starknet
 Home-page: https://github.com/Shard-Labs/starknet-devnet
 License: ISC
 Keywords: starknet,cairo,testnet,local,server
 Author: FabijanC
 Author-email: fabijan.corak@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask[async] (>=2.0.3,<2.1.0)
 Requires-Dist: Werkzeug (>=2.0.3,<2.1.0)
-Requires-Dist: cairo-lang (==0.11.0.1)
+Requires-Dist: cairo-lang (==0.11.0.2)
 Requires-Dist: cloudpickle (>=2.1.0,<2.2.0)
 Requires-Dist: crypto-cpp-py (>=1.2.0,<1.3.0)
 Requires-Dist: flask-cors (>=3.0.10,<3.1.0)
 Requires-Dist: gunicorn (>=20.1.0,<20.2.0)
 Requires-Dist: jsonschema (>=4.17.0,<4.18.0)
 Requires-Dist: marshmallow (>=3.17.0,<3.18.0)
 Requires-Dist: marshmallow-dataclass (>=8.4,<8.5)
 Requires-Dist: typing-extensions (>=4.3.0,<4.4.0)
-Requires-Dist: web3 (>=5.31.4,<5.32.0)
+Requires-Dist: web3 (>=6.0.0,<6.1.0)
 Project-URL: Repository, https://github.com/Shard-Labs/starknet-devnet
 Description-Content-Type: text/markdown
 
 <!-- logo / title -->
 <p align="center" style="margin-bottom: 0px !important">
   <img width="200" src="https://user-images.githubusercontent.com/2848732/193076972-da6fa36e-11f7-4cb3-aa29-673224f8576d.png" alt="Devnet" align="center">
 </p>
```

