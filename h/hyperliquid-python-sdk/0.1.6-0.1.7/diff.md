# Comparing `tmp/hyperliquid_python_sdk-0.1.6.tar.gz` & `tmp/hyperliquid_python_sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperliquid_python_sdk-0.1.6.tar", max compression
+gzip compressed data, was "hyperliquid_python_sdk-0.1.7.tar", max compression
```

## Comparing `hyperliquid_python_sdk-0.1.6.tar` & `hyperliquid_python_sdk-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2023-03-30 16:09:48.731040 hyperliquid_python_sdk-0.1.6/LICENSE.md
--rw-r--r--   0        0        0     5611 2023-03-30 17:53:30.856819 hyperliquid_python_sdk-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-03-20 20:28:58.636849 hyperliquid_python_sdk-0.1.6/hyperliquid/__init__.py
--rw-r--r--   0        0        0     1677 2023-03-30 17:02:32.596191 hyperliquid_python_sdk-0.1.6/hyperliquid/api.py
--rw-r--r--   0        0        0     3199 2023-03-30 17:02:32.596416 hyperliquid_python_sdk-0.1.6/hyperliquid/exchange.py
--rw-r--r--   0        0        0     4938 2023-03-30 17:02:32.596581 hyperliquid_python_sdk-0.1.6/hyperliquid/info.py
--rw-r--r--   0        0        0        0 2023-03-20 20:28:58.637272 hyperliquid_python_sdk-0.1.6/hyperliquid/utils/__init__.py
--rw-r--r--   0        0        0      144 2023-03-24 21:41:42.619628 hyperliquid_python_sdk-0.1.6/hyperliquid/utils/constants.py
--rw-r--r--   0        0        0      479 2023-03-20 20:28:58.637442 hyperliquid_python_sdk-0.1.6/hyperliquid/utils/error.py
--rw-r--r--   0        0        0     4927 2023-03-30 17:02:32.596872 hyperliquid_python_sdk-0.1.6/hyperliquid/utils/signing.py
--rw-r--r--   0        0        0     2174 2023-03-30 17:02:32.597142 hyperliquid_python_sdk-0.1.6/hyperliquid/utils/types.py
--rw-r--r--   0        0        0     4690 2023-03-30 17:02:32.597435 hyperliquid_python_sdk-0.1.6/hyperliquid/websocket_manager.py
--rw-r--r--   0        0        0     3838 2023-03-30 17:53:49.973257 hyperliquid_python_sdk-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     7199 1970-01-01 00:00:00.000000 hyperliquid_python_sdk-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-14 18:01:14.091628 hyperliquid_python_sdk-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0     5727 2023-04-14 18:01:14.101353 hyperliquid_python_sdk-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 18:01:14.086502 hyperliquid_python_sdk-0.1.7/hyperliquid/__init__.py
+-rw-r--r--   0        0        0     1677 2023-04-14 18:01:14.090826 hyperliquid_python_sdk-0.1.7/hyperliquid/api.py
+-rw-r--r--   0        0        0     3148 2023-04-14 18:01:14.086377 hyperliquid_python_sdk-0.1.7/hyperliquid/exchange.py
+-rw-r--r--   0        0        0     4938 2023-04-14 18:01:14.091061 hyperliquid_python_sdk-0.1.7/hyperliquid/info.py
+-rw-r--r--   0        0        0        0 2023-04-14 18:01:14.087711 hyperliquid_python_sdk-0.1.7/hyperliquid/utils/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-14 18:01:14.087641 hyperliquid_python_sdk-0.1.7/hyperliquid/utils/constants.py
+-rw-r--r--   0        0        0      479 2023-04-14 18:01:14.087371 hyperliquid_python_sdk-0.1.7/hyperliquid/utils/error.py
+-rw-r--r--   0        0        0     4927 2023-04-14 18:01:14.087022 hyperliquid_python_sdk-0.1.7/hyperliquid/utils/signing.py
+-rw-r--r--   0        0        0     2174 2023-04-14 18:01:14.087870 hyperliquid_python_sdk-0.1.7/hyperliquid/utils/types.py
+-rw-r--r--   0        0        0     4690 2023-04-14 18:01:14.091374 hyperliquid_python_sdk-0.1.7/hyperliquid/websocket_manager.py
+-rw-r--r--   0        0        0     3838 2023-04-14 18:04:41.692184 hyperliquid_python_sdk-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     7315 1970-01-01 00:00:00.000000 hyperliquid_python_sdk-0.1.7/PKG-INFO
```

### Comparing `hyperliquid_python_sdk-0.1.6/LICENSE.md` & `hyperliquid_python_sdk-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.1.6/README.md` & `hyperliquid_python_sdk-0.1.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/releases)
-[![License](https://img.shields.io/pypi/l/hyperliquid-python-sdk)](LICENSE.md)
-![Coverage Report](assets/images/coverage.svg)
+[![License](https://img.shields.io/pypi/l/hyperliquid-python-sdk)](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/blob/master/LICENSE.md)
+![Coverage Report](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/blob/master/assets/images/coverage.svg)
 
 SDK for Hyperliquid API trading with Python.
 
 </div>
 
 ## Installation
 ```bash
@@ -24,34 +24,34 @@
 from hyperliquid.info import Info
 from hyperliquid.utils import constants
 
 info = Info(constants.TESTNET_API_URL, skip_ws=True)
 user_state = info.user_state("0xcd5051944f780a621ee62e39e493c489668acf4d")
 print(user_state)
 ```
-See [examples](examples) for more complete examples. You can also checkout the repo and follow the developer setup and then run any of the examples e.g. `poetry run python examples/basic_order.py`
+See [examples](examples) for more complete examples. You can also checkout the repo and run any of the examples after configuring your private key e.g. 
+```bash
+cp examples/config.json.example examples/config.json
+vim examples/config.json
+python examples/basic_order.py
+```
+
 ## Getting started with development
 
 1. Download `Poetry`: https://python-poetry.org/. Note that in the install script you might have to set `symlinks=True` in `venv.EnvBuilder`.
 
 2. Point poetry to correct version of python. For development we require python 3.10 exactly. Some dependencies have issues on 3.11, while older versions don't have correct typing support.
 `brew install python@3.10 && poetry env use /opt/homebrew/Cellar/python@3.10/3.10.10_1/bin/python3.10`
 
 3. Install dependencies:
 
 ```bash
 make install
 ```
 
-4. Configure PYPI token to publish
-
-```bash
-poetry config pypi-token.pypi pypi-[your-token-here]
-```
-
 ### Makefile usage
 
 CLI commands for faster development.
 
 <details>
 <summary>Install all dependencies</summary>
 <p>
```

### Comparing `hyperliquid_python_sdk-0.1.6/hyperliquid/api.py` & `hyperliquid_python_sdk-0.1.7/hyperliquid/api.py`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.1.6/hyperliquid/exchange.py` & `hyperliquid_python_sdk-0.1.7/hyperliquid/exchange.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,17 +14,24 @@
     order_spec_to_order_wire,
     get_timestamp_ms,
 )
 from hyperliquid.utils.types import Meta, Any, Literal, Optional
 
 
 class Exchange(API):
-    def __init__(self, wallet: LocalAccount, base_url: Optional[str] = None, meta: Optional[Meta] = None):
+    def __init__(
+        self,
+        wallet: LocalAccount,
+        base_url: Optional[str] = None,
+        meta: Optional[Meta] = None,
+        vault_address: Optional[str] = None,
+    ):
         super().__init__(base_url)
         self.wallet = wallet
+        self.vault_address = vault_address
         if meta is None:
             info = Info(base_url, skip_ws=True)
             self.meta = info.meta()
         else:
             self.meta = meta
         self.coin_to_asset = {asset_info["name"]: asset for (asset, asset_info) in enumerate(self.meta["universe"])}
 
@@ -44,57 +51,50 @@
         timestamp = get_timestamp_ms()
         grouping: Literal["na"] = "na"
 
         signature = sign_l1_action(
             self.wallet,
             ["(uint32,bool,uint64,uint64,bool,uint8,uint64)[]", "uint8"],
             [[order_spec_preprocessing(order_spec)], order_grouping_to_number(grouping)],
-            ZERO_ADDRESS,
+            ZERO_ADDRESS if self.vault_address is None else self.vault_address,
             timestamp,
         )
-        logging.debug(
-            {
-                "action": {
-                    "type": "order",
-                    "grouping": grouping,
-                    "orders": [order_spec_to_order_wire(order_spec)],
-                },
-                "nonce": timestamp,
-                "signature": signature,
-                "vaultAddress": None,
-            }
-        )
-        return self.post(
-            "/exchange",
-            {
-                "action": {
-                    "type": "order",
-                    "grouping": grouping,
-                    "orders": [order_spec_to_order_wire(order_spec)],
-                },
-                "nonce": timestamp,
-                "signature": signature,
-                "vaultAddress": None,
+        payload = {
+            "action": {
+                "type": "order",
+                "grouping": grouping,
+                "orders": [order_spec_to_order_wire(order_spec)],
             },
-        )
+            "nonce": timestamp,
+            "signature": signature,
+            "vaultAddress": self.vault_address,
+        }
+        logging.debug(payload)
+        return self.post("/exchange", payload)
 
     def cancel(self, coin: str, oid: int) -> Any:
         timestamp = get_timestamp_ms()
         asset = self.coin_to_asset[coin]
-        signature = sign_l1_action(self.wallet, ["(uint32,uint64)[]"], [[(asset, oid)]], ZERO_ADDRESS, timestamp)
+        signature = sign_l1_action(
+            self.wallet,
+            ["(uint32,uint64)[]"],
+            [[(asset, oid)]],
+            ZERO_ADDRESS if self.vault_address is None else self.vault_address,
+            timestamp,
+        )
         return self.post(
             "/exchange",
             {
                 "action": {
                     "type": "cancel",
                     "cancels": [
                         {
                             "asset": asset,
                             "oid": oid,
                         }
                     ],
                 },
                 "nonce": timestamp,
                 "signature": signature,
-                "vaultAddress": None,
+                "vaultAddress": self.vault_address,
             },
         )
```

### Comparing `hyperliquid_python_sdk-0.1.6/hyperliquid/info.py` & `hyperliquid_python_sdk-0.1.7/hyperliquid/info.py`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.1.6/hyperliquid/utils/signing.py` & `hyperliquid_python_sdk-0.1.7/hyperliquid/utils/signing.py`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.1.6/hyperliquid/utils/types.py` & `hyperliquid_python_sdk-0.1.7/hyperliquid/utils/types.py`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.1.6/hyperliquid/websocket_manager.py` & `hyperliquid_python_sdk-0.1.7/hyperliquid/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.1.6/pyproject.toml` & `hyperliquid_python_sdk-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hyperliquid-python-sdk"
-version = "0.1.6"
+version = "0.1.7"
 description = "SDK for Hyperliquid API trading with Python."
 readme = "README.md"
 authors = ["Hyperliquid <hello@hyperliquid.xyz>"]
 license = "MIT"
 repository = "https://github.com/hyperliquid-dex/hyperliquid-python-sdk"
 homepage = "https://github.com/hyperliquid-dex/hyperliquid-python-sdk"
 packages = [
```

### Comparing `hyperliquid_python_sdk-0.1.6/PKG-INFO` & `hyperliquid_python_sdk-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperliquid-python-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: SDK for Hyperliquid API trading with Python.
 Home-page: https://github.com/hyperliquid-dex/hyperliquid-python-sdk
 License: MIT
 Author: Hyperliquid
 Author-email: hello@hyperliquid.xyz
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -40,16 +40,16 @@
 
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/releases)
-[![License](https://img.shields.io/pypi/l/hyperliquid-python-sdk)](LICENSE.md)
-![Coverage Report](assets/images/coverage.svg)
+[![License](https://img.shields.io/pypi/l/hyperliquid-python-sdk)](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/blob/master/LICENSE.md)
+![Coverage Report](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/blob/master/assets/images/coverage.svg)
 
 SDK for Hyperliquid API trading with Python.
 
 </div>
 
 ## Installation
 ```bash
@@ -60,34 +60,34 @@
 from hyperliquid.info import Info
 from hyperliquid.utils import constants
 
 info = Info(constants.TESTNET_API_URL, skip_ws=True)
 user_state = info.user_state("0xcd5051944f780a621ee62e39e493c489668acf4d")
 print(user_state)
 ```
-See [examples](examples) for more complete examples. You can also checkout the repo and follow the developer setup and then run any of the examples e.g. `poetry run python examples/basic_order.py`
+See [examples](examples) for more complete examples. You can also checkout the repo and run any of the examples after configuring your private key e.g. 
+```bash
+cp examples/config.json.example examples/config.json
+vim examples/config.json
+python examples/basic_order.py
+```
+
 ## Getting started with development
 
 1. Download `Poetry`: https://python-poetry.org/. Note that in the install script you might have to set `symlinks=True` in `venv.EnvBuilder`.
 
 2. Point poetry to correct version of python. For development we require python 3.10 exactly. Some dependencies have issues on 3.11, while older versions don't have correct typing support.
 `brew install python@3.10 && poetry env use /opt/homebrew/Cellar/python@3.10/3.10.10_1/bin/python3.10`
 
 3. Install dependencies:
 
 ```bash
 make install
 ```
 
-4. Configure PYPI token to publish
-
-```bash
-poetry config pypi-token.pypi pypi-[your-token-here]
-```
-
 ### Makefile usage
 
 CLI commands for faster development.
 
 <details>
 <summary>Install all dependencies</summary>
 <p>
```

