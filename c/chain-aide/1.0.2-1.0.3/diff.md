# Comparing `tmp/chain-aide-1.0.2.tar.gz` & `tmp/chain-aide-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chain-aide-1.0.2.tar", last modified: Wed Mar 29 10:01:04 2023, max compression
+gzip compressed data, was "chain-aide-1.0.3.tar", last modified: Fri Apr 14 06:56:02 2023, max compression
```

## Comparing `chain-aide-1.0.2.tar` & `chain-aide-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 10:01:04.121660 chain-aide-1.0.2/
--rw-rw-rw-   0        0        0     1083 2023-03-23 06:13:36.000000 chain-aide-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     3621 2023-03-29 10:01:04.121660 chain-aide-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2748 2023-03-23 09:11:09.000000 chain-aide-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-29 10:01:04.121660 chain-aide-1.0.2/chain_aide/
--rw-rw-rw-   0        0        0       65 2023-03-23 06:25:45.000000 chain-aide-1.0.2/chain_aide/__init__.py
--rw-rw-rw-   0        0        0     2528 2023-03-25 12:57:03.000000 chain-aide-1.0.2/chain_aide/contract.py
--rw-rw-rw-   0        0        0     8068 2023-03-25 13:47:31.000000 chain-aide-1.0.2/chain_aide/main.py
--rw-rw-rw-   0        0        0     1663 2023-03-25 14:04:58.000000 chain-aide-1.0.2/chain_aide/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-29 10:01:04.121660 chain-aide-1.0.2/chain_aide.egg-info/
--rw-rw-rw-   0        0        0     3621 2023-03-29 10:01:04.000000 chain-aide-1.0.2/chain_aide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-03-29 10:01:04.000000 chain-aide-1.0.2/chain_aide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 10:01:04.000000 chain-aide-1.0.2/chain_aide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-29 10:01:04.000000 chain-aide-1.0.2/chain_aide.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      174 2023-03-29 10:01:04.000000 chain-aide-1.0.2/chain_aide.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-29 10:01:04.000000 chain-aide-1.0.2/chain_aide.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-29 10:01:04.121660 chain-aide-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1620 2023-03-29 10:00:41.000000 chain-aide-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 06:56:02.220872 chain-aide-1.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-03-23 06:13:36.000000 chain-aide-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3589 2023-04-14 06:56:02.220872 chain-aide-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2716 2023-03-31 09:03:39.000000 chain-aide-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 06:56:02.215872 chain-aide-1.0.3/chain_aide/
+-rw-rw-rw-   0        0        0       65 2023-03-23 06:25:45.000000 chain-aide-1.0.3/chain_aide/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-03-31 06:26:42.000000 chain-aide-1.0.3/chain_aide/contract.py
+-rw-rw-rw-   0        0        0     6095 2023-03-31 06:21:32.000000 chain-aide-1.0.3/chain_aide/main.py
+-rw-rw-rw-   0        0        0     1635 2023-03-31 06:13:53.000000 chain-aide-1.0.3/chain_aide/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 06:56:02.219872 chain-aide-1.0.3/chain_aide.egg-info/
+-rw-rw-rw-   0        0        0     3589 2023-04-14 06:56:02.000000 chain-aide-1.0.3/chain_aide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-04-14 06:56:02.000000 chain-aide-1.0.3/chain_aide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 06:56:02.000000 chain-aide-1.0.3/chain_aide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 06:56:02.000000 chain-aide-1.0.3/chain_aide.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      174 2023-04-14 06:56:02.000000 chain-aide-1.0.3/chain_aide.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-14 06:56:02.000000 chain-aide-1.0.3/chain_aide.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 06:56:02.220872 chain-aide-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1620 2023-04-14 06:55:22.000000 chain-aide-1.0.3/setup.py
```

### Comparing `chain-aide-1.0.2/LICENSE` & `chain-aide-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chain-aide-1.0.2/PKG-INFO` & `chain-aide-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chain-aide
-Version: 1.0.2
+Version: 1.0.3
 Summary: An aide that helps you quickly access mainstream public chain and use its basic functions.
 Home-page: https://github.com/shinnng/chain-aide
 Author: Shinnng
 Author-email: shinnng@outlook.com
 License: MIT
 Keywords: chain
 Classifier: Development Status :: 4 - Beta
@@ -18,80 +18,78 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: chain-aide
 License-File: LICENSE
 
 # chain-aide
-它是一个能够帮助您快速访问各个主流区块链并使用其功能的小助手 
+它是一个能够帮助您快速访问各个主流区块链(目前仅支持eth)并使用其功能的小助手 
 
 
-# 安装方法
+## 安装方法
 ```shell
 pip install chain_aide
 ```
 
 
-# 使用方法
+## 使用方法
 
 ```python
 from eth_account import Account
 from chain_aide import Aide
 
 uri = 'http://192.168.120.121:6789'
 aide = Aide(uri)
+
+# 调用以太坊接口
 print(aide.web3.clientVersion)
 print(aide.web3.eth.block_number)
 
+# 设置默认账户  
+account = Account.from_key('f51ca759562e1daf9e5302d121f933a8152915d34fcbc27e542baf256b5e4b74')
+aide.set_default_account(account)
+
 """
 指定账户
 """
-# 使用默认账户发送交易，不需要再指定私钥
-account = Account.from_key('f51ca759562e1daf9e5302d121f933a8152915d34fcbc27e542baf256b5e4b74')
-aide.set_default_account(account)
+# 使用设置好的默认账户发送交易
 to_account = Account.create()
-print(aide.transfer.transfer(to_account.address, 10 * 10 ** 18))
+print(aide.transfer(to_account.address, 10 * 10 ** 18))
 
 # 使用私钥发送交易,比默认账户有更高的优先级
-txn = {'gas': 21000, 'gasPrice': 1 * 10 ** 9, 'nonce': 100}
 private_key = 'f51ca759562e1daf9e5302d121f933a8152915d34fcbc27e542baf256b5e4b74'
-print(aide.transfer.transfer(to_account.address, 10 * 10 ** 18, txn=txn, private_key=private_key))
+print(aide.transfer(to_account.address, 10 * 10 ** 18, private_key=private_key))
+
 
 """
-转账交易
+发送转账交易
 """
-# 发送转账
-to_account = Account.create(hrp='lat')
-print(aide.transfer.transfer(to_account.address, 10 * 10 ** 18))
+# 发送转账交易，自定义
+txn = {'gas': 21000, 'gasPrice': 1 * 10 ** 9, 'nonce': 100}
+to_account = Account.create()
+print(aide.transfer(to_account.address, 10 * 10 ** 18, txn=txn))
 
 """
-交易合约
+发送合约交易
 """
-false = False
-ture = True
-abi = [{"anonymous": false,
-        "inputs": [{"indexed": false, "internalType": "uint256", "name": "_chainId", "type": "uint256"}],
-        "name": "_putChainID", "type": "event"},
-       {"inputs": [], "name": "getChainID", "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
-        "stateMutability": "view", "type": "function"},
-       {"inputs": [], "name": "putChainID", "outputs": [], "stateMutability": "nonpayable", "type": "function"}]
+abi = [{"anonymous": False, "inputs": [{"indexed": False, "internalType": "uint256", "name": "_chainId", "type": "uint256"}], "name": "_putChainID", "type": "event"}, {"inputs": [], "name": "getChainID", "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}], "stateMutability": "view", "type": "function"}, {"inputs": [], "name": "putChainID", "outputs": [], "stateMutability": "nonpayable", "type": "function"}]
 bytecode = '608060405234801561001057600080fd5b50610107806100206000396000f3fe6080604052348015600f57600080fd5b506004361060325760003560e01c806336319ab0146037578063564b81ef14603f575b600080fd5b603d6059565b005b60456099565b6040516050919060ae565b60405180910390f35b466000819055507f68e891aec7f9596d6e192c48cb82364ec392d423bce80abd6e1ee5ad05860256600054604051608f919060ae565b60405180910390a1565b600046905090565b60a88160c7565b82525050565b600060208201905060c1600083018460a1565b92915050565b600081905091905056fea264697066735822122037a1668252253271128182c71109922cb1e300fb08a7080a0587f360df4071ba64736f6c63430008060033'
 
 # 部署新的合约
-contract = aide.contract.deploy(abi=abi, bytecode=bytecode)
+contract = aide.deploy_contract(abi=abi, bytecode=bytecode)
 print(contract.address)
 
 # 已有合约，直接初始化
-contract_address = '0x00'
-contract = aide.contract.init(abi=abi, address=contract_address)
+contract_address = '0x'
+contract = aide.init_contract(abi=abi, address=contract_address)
 print(contract.address)
 
 # call调用
-print(aide.contract.getChainID())
+print(contract.getChainID())
 
 # 发送交易(像call调用一样简答)
-res = aide.contract.putChainID()
+res = contract.putChainID()
 
 # 解析event
-print(aide.contract.PutChainID(res))
+print(contract.PutChainID(res))
 ```
```

### Comparing `chain-aide-1.0.2/README.md` & `chain-aide-1.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 # chain-aide
-它是一个能够帮助您快速访问各个主流区块链并使用其功能的小助手 
+它是一个能够帮助您快速访问各个主流区块链(目前仅支持eth)并使用其功能的小助手 
 
 
-# 安装方法
+## 安装方法
 ```shell
 pip install chain_aide
 ```
 
 
-# 使用方法
+## 使用方法
 
 ```python
 from eth_account import Account
 from chain_aide import Aide
 
 uri = 'http://192.168.120.121:6789'
 aide = Aide(uri)
+
+# 调用以太坊接口
 print(aide.web3.clientVersion)
 print(aide.web3.eth.block_number)
 
+# 设置默认账户  
+account = Account.from_key('f51ca759562e1daf9e5302d121f933a8152915d34fcbc27e542baf256b5e4b74')
+aide.set_default_account(account)
+
 """
 指定账户
 """
-# 使用默认账户发送交易，不需要再指定私钥
-account = Account.from_key('f51ca759562e1daf9e5302d121f933a8152915d34fcbc27e542baf256b5e4b74')
-aide.set_default_account(account)
+# 使用设置好的默认账户发送交易
 to_account = Account.create()
-print(aide.transfer.transfer(to_account.address, 10 * 10 ** 18))
+print(aide.transfer(to_account.address, 10 * 10 ** 18))
 
 # 使用私钥发送交易,比默认账户有更高的优先级
-txn = {'gas': 21000, 'gasPrice': 1 * 10 ** 9, 'nonce': 100}
 private_key = 'f51ca759562e1daf9e5302d121f933a8152915d34fcbc27e542baf256b5e4b74'
-print(aide.transfer.transfer(to_account.address, 10 * 10 ** 18, txn=txn, private_key=private_key))
+print(aide.transfer(to_account.address, 10 * 10 ** 18, private_key=private_key))
+
 
 """
-转账交易
+发送转账交易
 """
-# 发送转账
-to_account = Account.create(hrp='lat')
-print(aide.transfer.transfer(to_account.address, 10 * 10 ** 18))
+# 发送转账交易，自定义
+txn = {'gas': 21000, 'gasPrice': 1 * 10 ** 9, 'nonce': 100}
+to_account = Account.create()
+print(aide.transfer(to_account.address, 10 * 10 ** 18, txn=txn))
 
 """
-交易合约
+发送合约交易
 """
-false = False
-ture = True
-abi = [{"anonymous": false,
-        "inputs": [{"indexed": false, "internalType": "uint256", "name": "_chainId", "type": "uint256"}],
-        "name": "_putChainID", "type": "event"},
-       {"inputs": [], "name": "getChainID", "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
-        "stateMutability": "view", "type": "function"},
-       {"inputs": [], "name": "putChainID", "outputs": [], "stateMutability": "nonpayable", "type": "function"}]
+abi = [{"anonymous": False, "inputs": [{"indexed": False, "internalType": "uint256", "name": "_chainId", "type": "uint256"}], "name": "_putChainID", "type": "event"}, {"inputs": [], "name": "getChainID", "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}], "stateMutability": "view", "type": "function"}, {"inputs": [], "name": "putChainID", "outputs": [], "stateMutability": "nonpayable", "type": "function"}]
 bytecode = '608060405234801561001057600080fd5b50610107806100206000396000f3fe6080604052348015600f57600080fd5b506004361060325760003560e01c806336319ab0146037578063564b81ef14603f575b600080fd5b603d6059565b005b60456099565b6040516050919060ae565b60405180910390f35b466000819055507f68e891aec7f9596d6e192c48cb82364ec392d423bce80abd6e1ee5ad05860256600054604051608f919060ae565b60405180910390a1565b600046905090565b60a88160c7565b82525050565b600060208201905060c1600083018460a1565b92915050565b600081905091905056fea264697066735822122037a1668252253271128182c71109922cb1e300fb08a7080a0587f360df4071ba64736f6c63430008060033'
 
 # 部署新的合约
-contract = aide.contract.deploy(abi=abi, bytecode=bytecode)
+contract = aide.deploy_contract(abi=abi, bytecode=bytecode)
 print(contract.address)
 
 # 已有合约，直接初始化
-contract_address = '0x00'
-contract = aide.contract.init(abi=abi, address=contract_address)
+contract_address = '0x'
+contract = aide.init_contract(abi=abi, address=contract_address)
 print(contract.address)
 
 # call调用
-print(aide.contract.getChainID())
+print(contract.getChainID())
 
 # 发送交易(像call调用一样简答)
-res = aide.contract.putChainID()
+res = contract.putChainID()
 
 # 解析event
-print(aide.contract.PutChainID(res))
+print(contract.PutChainID(res))
 ```
```

### Comparing `chain-aide-1.0.2/chain_aide/contract.py` & `chain-aide-1.0.3/chain_aide/contract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-import warnings
-import sys
-from copy import copy
-
 from functools import wraps, partial
+from typing import TYPE_CHECKING
+
 from web3._utils.abi import filter_by_name
 from web3.contract.contract import ContractFunction
-from web3.types import ABI
-from eth_typing import HexStr, AnyAddress
 
 from chain_aide.utils import contract_call, contract_transaction
 
+if TYPE_CHECKING:
+    from chain_aide import Aide
+
 
 class Contract:
+    """ 简化合约操作
+    """
 
     def __init__(self,
-                 aide,
+                 aide: "Aide",
                  abi,
                  bytecode=None,
                  address=None,
                  ):
         self.aide = aide
         self.abi = abi
         self.bytecode = bytecode
@@ -27,14 +28,16 @@
         self.functions = self.origin.functions
         self.events = self.origin.events
         self._set_functions(self.origin.functions)
         self._set_events(self.origin.events)
         self._set_fallback(self.origin.fallback)
 
     def _set_functions(self, functions):
+        """ 包装合约方法，
+        """
         # 合约event和function不会重名，因此不用担心属性已存在
         for func in functions:
             warp_function = self._function_wrap(getattr(functions, func))
             setattr(self, func, warp_function)
 
     def _set_events(self, events):
         # 合约event和function不会重名，因此不用担心属性已存在
```

### Comparing `chain-aide-1.0.2/chain_aide/main.py` & `chain-aide-1.0.3/chain_aide/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 import time
 from typing import Literal
 
 from loguru import logger
-from web3.main import get_default_modules
 from web3.middleware import geth_poa_middleware
 from eth_account import Account
 from eth_account.signers.local import LocalAccount
-from eth_utils import to_checksum_address, combomethod
+from eth_utils import to_checksum_address, combomethod, remove_0x_prefix, to_canonical_address, keccak
 from chain_aide.contract import Contract
 from chain_aide.utils import get_web3
 
 
 class Aide:
-    """ 主类，功能如下：
-    1. 各个子模块的集合体，通过它来调用子模块发送交易
-    2. 持有设置数据，如：默认交易账户、经济模型数据、返回结果类型等
-    3. 包含一些常用方法，如：创建账户、等待块高/周期、区块解码等
+    """ 区块链接入助手，目前仅支持eth
     """
     transferGas: int = 21000
     account = Account()
 
     def __init__(self, uri: str):
         """
         Args:
-            uri: 节点开放的RPC链接
+            uri: 节点RPC链接
         """
         self.uri = uri
         self.default_account: LocalAccount = None  # 发送签名交易时适用的默认地址
         self.result_type = 'receipt'  # 交易返回的结果类型，包括：txn, hash, receipt
         # web3相关设置
         self.web3 = get_web3(uri)
         self.web3.middleware_onion.inject(geth_poa_middleware, layer=0)
@@ -140,20 +136,14 @@
 
         if not txn.get('from'):
             txn['from'] = account.address
 
         if not txn.get('nonce'):
             txn['nonce'] = self.eth.get_transaction_count(account.address)
 
-        # txn.pop('maxFeePerGas')
-        # txn.pop('maxPriorityFeePerGas')
-        # txn['gasPrice'] = self.web3.eth.gas_price
-        # txn['gas'] = 400000
-        print(f'txn: {txn}')
-
         signed_txn = self.eth.account.sign_transaction(txn, account.key)
         if result_type == "txn":
             return signed_txn
 
         tx_hash = self.eth.send_raw_transaction(signed_txn.rawTransaction)
         if result_type == 'hash':
             return tx_hash
@@ -161,20 +151,15 @@
         receipt = self.get_transaction_receipt(tx_hash)
         if result_type == 'receipt':
             return receipt
 
         raise ValueError(f'unknown result type {self.result_type}')
 
     def get_transaction_receipt(self, tx_hash, timeout=20):
-        """
-        发送签名交易，并根据结果类型获取交易结果
-
-        Args:
-            tx_hash: 要发送的交易dict
-            timeout:
+        """ 发送签名交易，并根据结果类型获取交易结果
         """
         receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=timeout)
         if type(receipt) is bytes:
             receipt = receipt.decode('utf-8')
 
         return receipt
 
@@ -193,33 +178,7 @@
 
             # 等待确定落链
             if current_block > to_block:
                 logger.info(f'waiting block: {current_block} -> {to_block}')
                 return
 
         raise TimeoutError('wait block timeout!')
-
-    # def ec_recover(self, block_identifier):
-    #     """ 使用keccak方式，解出区块的签名节点公钥
-    #     """
-    #     block = self.web3.eth.get_block(block_identifier)
-    #
-    #     extra = block.proofOfAuthorityData[:32]
-    #     sign = block.proofOfAuthorityData[32:]
-    #     raw_data = [bytes.fromhex(remove_0x_prefix(block.parentHash.hex())),
-    #                 to_canonical_address(block.miner),
-    #     #                 bytes.fromhex(remove_0x_prefix(block.stateRoot.hex())),
-    #                 bytes.fromhex(remove_0x_prefix(block.transactionsRoot.hex())),
-    #                 bytes.fromhex(remove_0x_prefix(block.receiptsRoot.hex())),
-    #                 bytes.fromhex(remove_0x_prefix(block.logsBloom.hex())),
-    #                 block.number,
-    #                 block.gasLimit,
-    #                 block.gasUsed,
-    #                 block.timestamp,
-    #                 extra,
-    #                 bytes.fromhex(remove_0x_prefix(block.nonce.hex()))
-    #                 ]
-    #     hash_bytes = HexBytes(keccak(rlp.encode(raw_data)))
-    #     signature_bytes = HexBytes(sign)
-    #     signature_bytes_standard = to_standard_signature_bytes(signature_bytes)
-    #     signature = Signature(signature_bytes=signature_bytes_standard)
-    #     return remove_0x_prefix(HexStr(signature.recover_public_key_from_msg_hash(hash_bytes).to_hex()))
```

### Comparing `chain-aide-1.0.2/chain_aide/utils.py` & `chain-aide-1.0.3/chain_aide/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,33 +23,32 @@
                 break
             t.sleep(1)
 
     return web3
 
 
 def contract_call(func):
+    """ 合约调用的包装类
+    """
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         return func(*args, **kwargs).call()
 
     return wrapper
 
 
-# 合约交易装饰器，仅用于接受参数
 def contract_transaction(func):
+    """ 合约交易的包装类
+    """
     @functools.wraps(func)
     def wrapper(self, *args, txn: dict = None, private_key=None, **kwargs):
-        """
-        """
         # 填充from地址，以免合约交易在预估gas时检验地址失败
         txn = txn or {}
-
         if not txn.get('from'):
             account = self.aide.eth.account.from_key(private_key, hrp=self.aide.hrp) if private_key else self.aide.default_account
             if account:
                 txn['from'] = account.address
 
-        # 构建合约交易体dict
         txn = func(*args, **kwargs).build_transaction(txn)
         return self.aide.send_transaction(txn, private_key=private_key)
 
     return wrapper
```

### Comparing `chain-aide-1.0.2/chain_aide.egg-info/PKG-INFO` & `chain-aide-1.0.3/chain_aide.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chain-aide
-Version: 1.0.2
+Version: 1.0.3
 Summary: An aide that helps you quickly access mainstream public chain and use its basic functions.
 Home-page: https://github.com/shinnng/chain-aide
 Author: Shinnng
 Author-email: shinnng@outlook.com
 License: MIT
 Keywords: chain
 Classifier: Development Status :: 4 - Beta
@@ -18,80 +18,78 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: chain-aide
 License-File: LICENSE
 
 # chain-aide
-它是一个能够帮助您快速访问各个主流区块链并使用其功能的小助手 
+它是一个能够帮助您快速访问各个主流区块链(目前仅支持eth)并使用其功能的小助手 
 
 
-# 安装方法
+## 安装方法
 ```shell
 pip install chain_aide
 ```
 
 
-# 使用方法
+## 使用方法
 
 ```python
 from eth_account import Account
 from chain_aide import Aide
 
 uri = 'http://192.168.120.121:6789'
 aide = Aide(uri)
+
+# 调用以太坊接口
 print(aide.web3.clientVersion)
 print(aide.web3.eth.block_number)
 
+# 设置默认账户  
+account = Account.from_key('f51ca759562e1daf9e5302d121f933a8152915d34fcbc27e542baf256b5e4b74')
+aide.set_default_account(account)
+
 """
 指定账户
 """
-# 使用默认账户发送交易，不需要再指定私钥
-account = Account.from_key('f51ca759562e1daf9e5302d121f933a8152915d34fcbc27e542baf256b5e4b74')
-aide.set_default_account(account)
+# 使用设置好的默认账户发送交易
 to_account = Account.create()
-print(aide.transfer.transfer(to_account.address, 10 * 10 ** 18))
+print(aide.transfer(to_account.address, 10 * 10 ** 18))
 
 # 使用私钥发送交易,比默认账户有更高的优先级
-txn = {'gas': 21000, 'gasPrice': 1 * 10 ** 9, 'nonce': 100}
 private_key = 'f51ca759562e1daf9e5302d121f933a8152915d34fcbc27e542baf256b5e4b74'
-print(aide.transfer.transfer(to_account.address, 10 * 10 ** 18, txn=txn, private_key=private_key))
+print(aide.transfer(to_account.address, 10 * 10 ** 18, private_key=private_key))
+
 
 """
-转账交易
+发送转账交易
 """
-# 发送转账
-to_account = Account.create(hrp='lat')
-print(aide.transfer.transfer(to_account.address, 10 * 10 ** 18))
+# 发送转账交易，自定义
+txn = {'gas': 21000, 'gasPrice': 1 * 10 ** 9, 'nonce': 100}
+to_account = Account.create()
+print(aide.transfer(to_account.address, 10 * 10 ** 18, txn=txn))
 
 """
-交易合约
+发送合约交易
 """
-false = False
-ture = True
-abi = [{"anonymous": false,
-        "inputs": [{"indexed": false, "internalType": "uint256", "name": "_chainId", "type": "uint256"}],
-        "name": "_putChainID", "type": "event"},
-       {"inputs": [], "name": "getChainID", "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
-        "stateMutability": "view", "type": "function"},
-       {"inputs": [], "name": "putChainID", "outputs": [], "stateMutability": "nonpayable", "type": "function"}]
+abi = [{"anonymous": False, "inputs": [{"indexed": False, "internalType": "uint256", "name": "_chainId", "type": "uint256"}], "name": "_putChainID", "type": "event"}, {"inputs": [], "name": "getChainID", "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}], "stateMutability": "view", "type": "function"}, {"inputs": [], "name": "putChainID", "outputs": [], "stateMutability": "nonpayable", "type": "function"}]
 bytecode = '608060405234801561001057600080fd5b50610107806100206000396000f3fe6080604052348015600f57600080fd5b506004361060325760003560e01c806336319ab0146037578063564b81ef14603f575b600080fd5b603d6059565b005b60456099565b6040516050919060ae565b60405180910390f35b466000819055507f68e891aec7f9596d6e192c48cb82364ec392d423bce80abd6e1ee5ad05860256600054604051608f919060ae565b60405180910390a1565b600046905090565b60a88160c7565b82525050565b600060208201905060c1600083018460a1565b92915050565b600081905091905056fea264697066735822122037a1668252253271128182c71109922cb1e300fb08a7080a0587f360df4071ba64736f6c63430008060033'
 
 # 部署新的合约
-contract = aide.contract.deploy(abi=abi, bytecode=bytecode)
+contract = aide.deploy_contract(abi=abi, bytecode=bytecode)
 print(contract.address)
 
 # 已有合约，直接初始化
-contract_address = '0x00'
-contract = aide.contract.init(abi=abi, address=contract_address)
+contract_address = '0x'
+contract = aide.init_contract(abi=abi, address=contract_address)
 print(contract.address)
 
 # call调用
-print(aide.contract.getChainID())
+print(contract.getChainID())
 
 # 发送交易(像call调用一样简答)
-res = aide.contract.putChainID()
+res = contract.putChainID()
 
 # 解析event
-print(aide.contract.PutChainID(res))
+print(contract.PutChainID(res))
 ```
```

### Comparing `chain-aide-1.0.2/setup.py` & `chain-aide-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with open('./README.md', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='chain-aide',
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version='1.0.2',
+    version='1.0.3',
     description="""An aide that helps you quickly access mainstream public chain and use its basic functions.""",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Shinnng',
     author_email='shinnng@outlook.com',
     url='https://github.com/shinnng/chain-aide',
     include_package_data=True,
```

