# Comparing `tmp/symbol-sdk-python-3.0.3.tar.gz` & `tmp/symbol-sdk-python-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbol-sdk-python-3.0.3.tar", max compression
+gzip compressed data, was "symbol-sdk-python-3.0.5.tar", max compression
```

## Comparing `symbol-sdk-python-3.0.3.tar` & `symbol-sdk-python-3.0.5.tar`

### file list

```diff
@@ -1,46 +1,55 @@
--rw-r--r--   0        0        0      353 2022-03-15 13:17:51.315781 symbol-sdk-python-3.0.3/README.md
--rw-r--r--   0        0        0      630 2022-03-15 13:24:31.523457 symbol-sdk-python-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     2508 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/AccountDescriptorRepository.py
--rw-r--r--   0        0        0     3728 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/ArrayHelpers.py
--rw-r--r--   0        0        0     1482 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/BaseValue.py
--rw-r--r--   0        0        0     1611 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/Bip32.py
--rw-r--r--   0        0        0      723 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/BlockchainSettings.py
--rw-r--r--   0        0        0      883 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/BufferReader.py
--rw-r--r--   0        0        0      639 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/BufferWriter.py
--rw-r--r--   0        0        0     1059 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/ByteArray.py
--rw-r--r--   0        0        0     1233 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/CodeWordsEncoder.py
--rw-r--r--   0        0        0     1314 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/CryptoTypes.py
--rw-r--r--   0        0        0     1848 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/DiceMnemonicGenerator.py
--rw-r--r--   0        0        0     2406 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/Network.py
--rw-r--r--   0        0        0     1594 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/NetworkTimestamp.py
--rw-r--r--   0        0        0     1019 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/NodeDescriptorRepository.py
--rw-r--r--   0        0        0      397 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/Ordered.py
--rw-r--r--   0        0        0     1606 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/PrivateKeyStorage.py
--rw-r--r--   0        0        0     1348 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/QrSignatureStorage.py
--rw-r--r--   0        0        0     1494 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/QrStorage.py
--rw-r--r--   0        0        0     4992 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/RuleBasedTransactionFactory.py
--rw-r--r--   0        0        0     1707 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/TransactionDescriptorProcessor.py
--rw-r--r--   0        0        0        0 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/__init__.py
--rw-r--r--   0        0        0     2983 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/facade/BatchOperations.py
--rw-r--r--   0        0        0     2481 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/facade/NemFacade.py
--rw-r--r--   0        0        0     4108 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/facade/SymbolFacade.py
--rw-r--r--   0        0        0        0 2022-03-15 13:17:51.319781 symbol-sdk-python-3.0.3/symbolchain/facade/__init__.py
--rw-r--r--   0        0        0   170406 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/nc/__init__.py
--rw-r--r--   0        0        0     1155 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/nem/KeyPair.py
--rw-r--r--   0        0        0      938 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/nem/Network.py
--rw-r--r--   0        0        0      876 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/nem/NetworkTimestamp.py
--rw-r--r--   0        0        0     3459 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/nem/TransactionFactory.py
--rw-r--r--   0        0        0        0 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/nem/__init__.py
--rw-r--r--   0        0        0        0 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/nem/external/__init__.py
--rw-r--r--   0        0        0     7006 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/nem/external/ed25519.py
--rw-r--r--   0        0        0   352662 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/sc/__init__.py
--rw-r--r--   0        0        0     1687 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/symbol/IdGenerator.py
--rw-r--r--   0        0        0     1420 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/symbol/KeyPair.py
--rw-r--r--   0        0        0      941 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/symbol/MerkleHashBuilder.py
--rw-r--r--   0        0        0     1416 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/symbol/Network.py
--rw-r--r--   0        0        0     1043 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/symbol/NetworkTimestamp.py
--rw-r--r--   0        0        0     2799 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/symbol/TransactionFactory.py
--rw-r--r--   0        0        0     1347 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/symbol/VotingKeysGenerator.py
--rw-r--r--   0        0        0        0 2022-03-15 13:17:51.323781 symbol-sdk-python-3.0.3/symbolchain/symbol/__init__.py
--rw-r--r--   0        0        0     1298 2022-03-15 13:24:36.901268 symbol-sdk-python-3.0.3/setup.py
--rw-r--r--   0        0        0     1357 2022-03-15 13:24:36.901547 symbol-sdk-python-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0      353 2023-04-14 01:07:43.302860 symbol-sdk-python-3.0.5/README.md
+-rw-r--r--   0        0        0      674 2023-04-14 05:56:51.040702 symbol-sdk-python-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2508 2023-04-14 01:07:43.302860 symbol-sdk-python-3.0.5/symbolchain/AccountDescriptorRepository.py
+-rw-r--r--   0        0        0     3728 2023-04-14 01:07:43.302860 symbol-sdk-python-3.0.5/symbolchain/ArrayHelpers.py
+-rw-r--r--   0        0        0     1482 2023-04-14 01:07:43.302860 symbol-sdk-python-3.0.5/symbolchain/BaseValue.py
+-rw-r--r--   0        0        0     1787 2023-04-14 01:07:43.302860 symbol-sdk-python-3.0.5/symbolchain/Bip32.py
+-rw-r--r--   0        0        0      723 2023-04-14 01:07:43.302860 symbol-sdk-python-3.0.5/symbolchain/BlockchainSettings.py
+-rw-r--r--   0        0        0      883 2023-04-14 01:07:43.302860 symbol-sdk-python-3.0.5/symbolchain/BufferReader.py
+-rw-r--r--   0        0        0      639 2023-04-14 01:07:43.302860 symbol-sdk-python-3.0.5/symbolchain/BufferWriter.py
+-rw-r--r--   0        0        0     1059 2023-04-14 01:07:43.302860 symbol-sdk-python-3.0.5/symbolchain/ByteArray.py
+-rw-r--r--   0        0        0     2158 2023-04-14 01:07:43.302860 symbol-sdk-python-3.0.5/symbolchain/Cipher.py
+-rw-r--r--   0        0        0     1233 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/CodeWordsEncoder.py
+-rw-r--r--   0        0        0     1844 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/CryptoTypes.py
+-rw-r--r--   0        0        0     1848 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/DiceMnemonicGenerator.py
+-rw-r--r--   0        0        0     3368 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/Network.py
+-rw-r--r--   0        0        0     1594 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/NetworkTimestamp.py
+-rw-r--r--   0        0        0     1019 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/NodeDescriptorRepository.py
+-rw-r--r--   0        0        0      397 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/Ordered.py
+-rw-r--r--   0        0        0     1606 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/PrivateKeyStorage.py
+-rw-r--r--   0        0        0     1348 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/QrSignatureStorage.py
+-rw-r--r--   0        0        0     1494 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/QrStorage.py
+-rw-r--r--   0        0        0     4992 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/RuleBasedTransactionFactory.py
+-rw-r--r--   0        0        0      593 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/SharedKey.py
+-rw-r--r--   0        0        0     1809 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/TransactionDescriptorProcessor.py
+-rw-r--r--   0        0        0      226 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/Transforms.py
+-rw-r--r--   0        0        0        0 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/external/__init__.py
+-rw-r--r--   0        0        0     7833 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/external/ed25519.py
+-rw-r--r--   0        0        0     2983 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/facade/BatchOperations.py
+-rw-r--r--   0        0        0     2801 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/facade/NemFacade.py
+-rw-r--r--   0        0        0     4940 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/facade/SymbolFacade.py
+-rw-r--r--   0        0        0        0 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/facade/__init__.py
+-rw-r--r--   0        0        0     2152 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/impl/CipherHelpers.py
+-rw-r--r--   0        0        0        0 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/impl/__init__.py
+-rw-r--r--   0        0        0   178806 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/nc/__init__.py
+-rw-r--r--   0        0        0     3712 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/nem/KeyPair.py
+-rw-r--r--   0        0        0     2374 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/nem/MessageEncoder.py
+-rw-r--r--   0        0        0     1746 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/nem/Network.py
+-rw-r--r--   0        0        0     1094 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/nem/SharedKey.py
+-rw-r--r--   0        0        0     3748 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/nem/TransactionFactory.py
+-rw-r--r--   0        0        0        0 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/nem/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-14 01:07:43.306860 symbol-sdk-python-3.0.5/symbolchain/ripemd160.py
+-rw-r--r--   0        0        0   477679 2023-04-14 01:07:43.310860 symbol-sdk-python-3.0.5/symbolchain/sc/__init__.py
+-rw-r--r--   0        0        0     1696 2023-04-14 01:07:43.310860 symbol-sdk-python-3.0.5/symbolchain/symbol/IdGenerator.py
+-rw-r--r--   0        0        0     1506 2023-04-14 01:07:43.310860 symbol-sdk-python-3.0.5/symbolchain/symbol/KeyPair.py
+-rw-r--r--   0        0        0     7243 2023-04-14 01:07:43.310860 symbol-sdk-python-3.0.5/symbolchain/symbol/Merkle.py
+-rw-r--r--   0        0        0     2476 2023-04-14 01:07:43.310860 symbol-sdk-python-3.0.5/symbolchain/symbol/MessageEncoder.py
+-rw-r--r--   0        0        0      567 2023-04-14 01:07:43.310860 symbol-sdk-python-3.0.5/symbolchain/symbol/Metadata.py
+-rw-r--r--   0        0        0     2229 2023-04-14 01:07:43.310860 symbol-sdk-python-3.0.5/symbolchain/symbol/Network.py
+-rw-r--r--   0        0        0      334 2023-04-14 01:07:43.310860 symbol-sdk-python-3.0.5/symbolchain/symbol/SharedKey.py
+-rw-r--r--   0        0        0     3355 2023-04-14 01:07:43.310860 symbol-sdk-python-3.0.5/symbolchain/symbol/TransactionFactory.py
+-rw-r--r--   0        0        0     1686 2023-04-14 01:07:43.310860 symbol-sdk-python-3.0.5/symbolchain/symbol/VotingKeysGenerator.py
+-rw-r--r--   0        0        0        0 2023-04-14 01:07:43.310860 symbol-sdk-python-3.0.5/symbolchain/symbol/__init__.py
+-rw-r--r--   0        0        0     1361 2023-04-14 05:56:52.890843 symbol-sdk-python-3.0.5/setup.py
+-rw-r--r--   0        0        0     1431 2023-04-14 05:56:52.891217 symbol-sdk-python-3.0.5/PKG-INFO
```

### Comparing `symbol-sdk-python-3.0.3/pyproject.toml` & `symbol-sdk-python-3.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'symbol-sdk-python'
-version = '3.0.3'
+version = '3.0.5'
 description = 'Symbol SDK'
 authors = ['Symbol Contributors <contributors@symbol.dev>']
 maintainers = ['Symbol Contributors <contributors@symbol.dev>']
 license = 'MIT'
 
 readme = 'README.md'
 
@@ -14,14 +14,16 @@
 
 keywords = ['symbol', 'sdk', 'Symbol SDK']
 
 classifiers = ['Programming Language :: Python :: 3.7']
 
 [tool.poetry.dependencies]
 python = "^3.7"
-cryptography = "36.0.1"
+cryptography = "40.0.1"
 mnemonic = "0.20"
-Pillow = "9.0.1"
-pysha3 = "1.0.2"
+Pillow = "9.5.0"
+PyNaCl = "1.5.0"
 PyYAML = "6.0"
-pyzbar = "0.1.8"
-qrcode = "7.3.1"
+pyzbar = "0.1.9"
+qrcode = "7.4.2"
+ripemd-hash = "1.0.0"
+safe-pysha3 = "1.0.3"
```

### Comparing `symbol-sdk-python-3.0.3/symbolchain/AccountDescriptorRepository.py` & `symbol-sdk-python-3.0.5/symbolchain/AccountDescriptorRepository.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/ArrayHelpers.py` & `symbol-sdk-python-3.0.5/symbolchain/ArrayHelpers.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/BaseValue.py` & `symbol-sdk-python-3.0.5/symbolchain/BaseValue.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/Bip32.py` & `symbol-sdk-python-3.0.5/symbolchain/Bip32.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import hashlib
 import hmac
+import secrets
 
 from mnemonic import Mnemonic
 
 from .BufferWriter import BufferWriter
 from .CryptoTypes import PrivateKey
 
 
-class Bip32Node():
+class Bip32Node:
 	"""Representation of a BIP32 node."""
 
 	def __init__(self, hmac_key, data):
 		"""Creates a BIP32 node around a key and data."""
 		hmac_result = hmac.new(hmac_key, data, hashlib.sha512).digest()
 
 		self.private_key = PrivateKey(hmac_result[0:PrivateKey.SIZE])
@@ -30,22 +31,26 @@
 		next_node = self
 		for identifier in path:
 			next_node = next_node.derive_one(identifier)
 
 		return next_node
 
 
-class Bip32():
+class Bip32:
 	"""Factory of BIP32 root nodes """
 
 	def __init__(self, curve_name='ed25519', mnemonic_language='english'):
 		"""Creates a BIP32 root node factory."""
 		self.root_hmac_key = (curve_name + ' seed').encode('utf8')
 		self.mnemonic_language = mnemonic_language
 
 	def from_seed(self, seed):
 		"""Creates a BIP32 root node from a seed."""
 		return Bip32Node(self.root_hmac_key, seed)
 
 	def from_mnemonic(self, mnemonic, password):
 		"""Creates a BIP32 root node from a BIP39 mnemonic and password."""
 		return self.from_seed(Mnemonic(self.mnemonic_language).to_seed(mnemonic, password))
+
+	def random(self, seed_length=32):
+		"""Creates a random BIP32 mnemonic."""
+		return Mnemonic(self.mnemonic_language).to_mnemonic(secrets.token_bytes(seed_length))
```

### Comparing `symbol-sdk-python-3.0.3/symbolchain/BlockchainSettings.py` & `symbol-sdk-python-3.0.5/symbolchain/BlockchainSettings.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/BufferReader.py` & `symbol-sdk-python-3.0.5/symbolchain/BufferReader.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/BufferWriter.py` & `symbol-sdk-python-3.0.5/symbolchain/BufferWriter.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/ByteArray.py` & `symbol-sdk-python-3.0.5/symbolchain/ByteArray.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/CodeWordsEncoder.py` & `symbol-sdk-python-3.0.5/symbolchain/CodeWordsEncoder.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/CryptoTypes.py` & `symbol-sdk-python-3.0.5/symbolchain/CryptoTypes.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 	SIZE = 32
 
 	def __init__(self, hash256):
 		"""Creates a hash from bytes or a hex string."""
 		super().__init__(self.SIZE, hash256, Hash256)
 
+	def __repr__(self):
+		return f'Hash256(\'{str(self)}\')'
+
 	@staticmethod
 	def zero():
 		"""Creates a zeroed hash."""
 		return Hash256(bytes([0] * Hash256.SIZE))
 
 
 class PrivateKey(ByteArray):
@@ -23,14 +26,17 @@
 
 	SIZE = 32
 
 	def __init__(self, private_key):
 		"""Creates a private key from bytes or a hex string."""
 		super().__init__(self.SIZE, private_key, PrivateKey)
 
+	def __repr__(self):
+		return f'PrivateKey(\'{str(self)}\')'
+
 	@staticmethod
 	def random():
 		"""Generates a random private key."""
 		return PrivateKey(secrets.token_bytes(PrivateKey.SIZE))
 
 
 class PublicKey(ByteArray):
@@ -38,21 +44,40 @@
 
 	SIZE = 32
 
 	def __init__(self, public_key):
 		"""Creates a public key from bytes or a hex string."""
 		super().__init__(self.SIZE, public_key.bytes if isinstance(public_key, PublicKey) else public_key, PublicKey)
 
+	def __repr__(self):
+		return f'PublicKey(\'{str(self)}\')'
+
+
+class SharedKey256(ByteArray):
+	"""Represents 256-bit symmetric encryption key."""
+
+	SIZE = 32
+
+	def __init__(self, key):
+		"""Creates a key from bytes or a hex string."""
+		super().__init__(self.SIZE, key, SharedKey256)
+
+	def __repr__(self):
+		return f'SharedKey256(\'{str(self)}\')'
+
 
 class Signature(ByteArray):
 	"""Represents a signature."""
 
 	SIZE = 64
 
 	def __init__(self, signature):
 		"""Creates a signature from bytes or a hex string."""
 		super().__init__(self.SIZE, signature, Signature)
 
+	def __repr__(self):
+		return f'Signature(\'{str(self)}\')'
+
 	@staticmethod
 	def zero():
 		"""Creates a zeroed signature."""
 		return Signature(bytes([0] * Signature.SIZE))
```

### Comparing `symbol-sdk-python-3.0.3/symbolchain/DiceMnemonicGenerator.py` & `symbol-sdk-python-3.0.5/symbolchain/DiceMnemonicGenerator.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/Network.py` & `symbol-sdk-python-3.0.5/symbolchain/Network.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,74 @@
-import hashlib
 from abc import abstractmethod
 
+from symbolchain.ripemd160 import ripemd160
+
+BASE32_RFC4648_ALPHABET = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ234567'
+
 
 class Network:
 	"""Represents a network."""
 
-	def __init__(self, name, identifier):
-		"""Creates a new network with the specified name and identifier byte."""
+	def __init__(self, name, identifier, datetime_converter, address_class, network_timestamp_class):
+		# pylint: disable=too-many-arguments
+
+		"""Creates a new network with the specified properties."""
 		self.name = name
 		self.identifier = identifier
+		self.datetime_converter = datetime_converter
+
+		self.address_class = address_class
+		self.network_timestamp_class = network_timestamp_class
 
 	def public_key_to_address(self, public_key):
 		"""Converts a public key to an address."""
 		part_one_hash_builder = self.address_hasher()
 		part_one_hash_builder.update(public_key.bytes)
 		part_one_hash = part_one_hash_builder.digest()
 
-		part_two_hash_builder = hashlib.new('ripemd160')
-		part_two_hash_builder.update(part_one_hash)
-		part_two_hash = part_two_hash_builder.digest()
+		part_two_hash = ripemd160(part_one_hash)
 
 		version = bytes([self.identifier]) + part_two_hash
 
 		part_three_hash_builder = self.address_hasher()
 		part_three_hash_builder.update(version)
 		checksum = part_three_hash_builder.digest()[0:4]
 
 		return self.create_address(version, checksum)
 
+	def is_valid_address_string(self, address_string):
+		"""Checks if an address string is valid and belongs to this network."""
+		if self.address_class.ENCODED_SIZE != len(address_string):
+			return False
+
+		if any(ch not in BASE32_RFC4648_ALPHABET for ch in address_string):
+			return False
+
+		return self.is_valid_address(self.address_class(address_string))
+
 	def is_valid_address(self, address):
 		"""Checks if an address is valid and belongs to this network."""
 		if address.bytes[0] != self.identifier:
 			return False
 
 		hash_builder = self.address_hasher()
 		hash_builder.update(address.bytes[0:1 + 20])
 
 		checksum_from_address = address.bytes[1 + 20:]
 		calculated_checksum = hash_builder.digest()[0:len(checksum_from_address)]
 		return checksum_from_address == calculated_checksum
 
+	def to_datetime(self, reference_network_timestamp):
+		"""Converts a network timestamp to a datetime."""
+		return self.datetime_converter.to_datetime(reference_network_timestamp.timestamp)
+
+	def from_datetime(self, reference_datetime):
+		"""Converts a datetime to a network timestamp."""
+		return self.network_timestamp_class(self.datetime_converter.to_difference(reference_datetime))
+
 	@abstractmethod
 	def address_hasher(self):
 		"""Gets the primary hasher to use in the public key to address conversion."""
 
 	@abstractmethod
 	def create_address(self, address_without_checksum, checksum):
 		"""Creates an encoded address from an address without checksum and checksum bytes."""
```

### Comparing `symbol-sdk-python-3.0.3/symbolchain/NetworkTimestamp.py` & `symbol-sdk-python-3.0.5/symbolchain/NetworkTimestamp.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/NodeDescriptorRepository.py` & `symbol-sdk-python-3.0.5/symbolchain/NodeDescriptorRepository.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/PrivateKeyStorage.py` & `symbol-sdk-python-3.0.5/symbolchain/PrivateKeyStorage.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/QrSignatureStorage.py` & `symbol-sdk-python-3.0.5/symbolchain/QrSignatureStorage.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/QrStorage.py` & `symbol-sdk-python-3.0.5/symbolchain/QrStorage.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/RuleBasedTransactionFactory.py` & `symbol-sdk-python-3.0.5/symbolchain/RuleBasedTransactionFactory.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/TransactionDescriptorProcessor.py` & `symbol-sdk-python-3.0.5/symbolchain/TransactionDescriptorProcessor.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 
 	def copy_to(self, transaction, ignore_keys=None):
 		"""Copies all descriptor information to a transaction."""
 		for key in self.transaction_descriptor.keys():
 			if ignore_keys and key in ignore_keys:
 				continue
 
+			if key.endswith('_computed'):
+				raise ValueError(f'cannot explicitly set computed field {key}')
+
 			if not hasattr(transaction, key):
 				raise ValueError(f'transaction does not have attribute {key}')
 
 			value = self.lookup_value(key)
 			if isinstance(value, list):
 				getattr(transaction, key).extend(value)
 			else:
```

### Comparing `symbol-sdk-python-3.0.3/symbolchain/facade/BatchOperations.py` & `symbol-sdk-python-3.0.5/symbolchain/facade/BatchOperations.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.3/symbolchain/facade/NemFacade.py` & `symbol-sdk-python-3.0.5/symbolchain/facade/NemFacade.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import sha3
 
 from ..CryptoTypes import Hash256, PrivateKey, PublicKey
 from ..nem.KeyPair import KeyPair, Verifier
 from ..nem.Network import Address, Network
+from ..nem.SharedKey import SharedKey
 from ..nem.TransactionFactory import TransactionFactory
 from ..Network import NetworkLocator
 
 
 class NemFacade:
 	"""Facade used to interact with NEM blockchain."""
 
-	BIP32_COIN_ID = 43
 	BIP32_CURVE_NAME = 'ed25519-keccak'
 
-	Address = Address
-	KeyPair = KeyPair
+	Address = Address  # pylint: disable=duplicate-code
+	KeyPair = KeyPair  # pylint: disable=duplicate-code
 	Verifier = Verifier
+	SharedKey = SharedKey
 
-	def __init__(self, nem_network_name, account_descriptor_repository=None):
+	def __init__(self, network, account_descriptor_repository=None):
 		"""Creates a NEM facade."""
-		self.network = NetworkLocator.find_by_name(Network.NETWORKS, nem_network_name)
+		self.network = NetworkLocator.find_by_name(Network.NETWORKS, network) if isinstance(network, str) else network
 		self.account_descriptor_repository = account_descriptor_repository
 		self.transaction_factory = self._create_nem_transaction_factory()
 
 	def _create_nem_transaction_factory(self):
 		type_parsing_rules = None
 		if self.account_descriptor_repository:
 			type_parsing_rules = self.account_descriptor_repository.to_type_parsing_rules_map(self._create_nem_type_to_property_mapping())
@@ -53,12 +54,16 @@
 
 	@staticmethod
 	def verify_transaction(transaction, signature):
 		"""Verifies a NEM transaction."""
 		non_verifiable_transaction = TransactionFactory.to_non_verifiable_transaction(transaction)
 		return Verifier(transaction.signer_public_key).verify(non_verifiable_transaction.serialize(), signature)
 
+	def bip32_path(self, account_id):
+		"""Creates a network compatible BIP32 path for the specified account."""
+		return [44, 43 if 'mainnet' == self.network.name else 1, account_id, 0, 0]
+
 	@staticmethod
 	def bip32_node_to_key_pair(bip32_node):
 		"""Derives a NEM KeyPair from a BIP32 node."""
 		# BIP32 private keys should be used as is, so reverse here to counteract reverse in KeyPair
 		return KeyPair(PrivateKey(bip32_node.private_key.bytes[::-1]))
```

### Comparing `symbol-sdk-python-3.0.3/symbolchain/facade/SymbolFacade.py` & `symbol-sdk-python-3.0.5/symbolchain/symbol/TransactionFactory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,109 +1,90 @@
-import sha3
+from binascii import hexlify
 
-from ..CryptoTypes import Hash256, PublicKey, Signature
-from ..Network import NetworkLocator
-from ..sc import TransactionType
-from ..symbol.KeyPair import KeyPair, Verifier
-from ..symbol.MerkleHashBuilder import MerkleHashBuilder
-from ..symbol.Network import Address, Network
-from ..symbol.TransactionFactory import TransactionFactory
-
-TRANSACTION_HEADER_SIZE = sum(field[1] for field in [
-	('size', 4),
-	('reserved1', 4),
-	('signature', Signature.SIZE),
-	('signer', PublicKey.SIZE),
-	('reserved2', 4)
-])
-
-AGGREGATE_HASHED_SIZE = sum(field[1] for field in [
-	('version_network_type', 4),
-	('max_fee', 8),
-	('deadline', 8),
-	('transactions_hash', Hash256.SIZE)
-])
-
-
-class SymbolFacade:
-	"""Facade used to interact with Symbol blockchain."""
-
-	BIP32_COIN_ID = 4343
-	BIP32_CURVE_NAME = 'ed25519'
-
-	Address = Address
-	KeyPair = KeyPair
-	Verifier = Verifier
-
-	def __init__(self, symbol_network_name, account_descriptor_repository=None):
-		"""Creates a Symbol facade."""
-		self.network = NetworkLocator.find_by_name(Network.NETWORKS, symbol_network_name)
-		self.account_descriptor_repository = account_descriptor_repository
-		self.transaction_factory = self._create_symbol_transaction_factory()
-
-	def _create_symbol_transaction_factory(self):
-		type_parsing_rules = None
-		if self.account_descriptor_repository:
-			type_to_property_mapping = self._create_symbol_type_to_property_mapping()
-			type_parsing_rules = self.account_descriptor_repository.to_type_parsing_rules_map(type_to_property_mapping)
+from symbolchain import sc
 
-		return TransactionFactory(self.network, type_parsing_rules)
+from ..CryptoTypes import Hash256, PublicKey
+from ..RuleBasedTransactionFactory import RuleBasedTransactionFactory
+from .IdGenerator import generate_mosaic_id, generate_namespace_id
+from .Network import Address
+
+
+class TransactionFactory:
+	"""Factory for creating Symbol transactions."""
+
+	def __init__(self, network, type_rule_overrides=None):
+		"""Creates a factory for the specified network."""
+		self.factory = self._build_rules(type_rule_overrides)
+		self.network = network
+
+	def _create_and_extend(self, transaction_descriptor, autosort, factory_class):
+		transaction = self.factory.create_from_factory(factory_class.create_by_name, {
+			**transaction_descriptor,
+			'network': self.network.identifier
+		})
+		if autosort:
+			transaction.sort()
+
+		# autogenerate artifact ids
+		if sc.TransactionType.NAMESPACE_REGISTRATION == transaction.type_:
+			parent_id = transaction.parent_id.value if sc.NamespaceRegistrationType.CHILD == transaction.registration_type else 0
+			transaction.id = sc.NamespaceId(generate_namespace_id(transaction.name.decode('utf8'), parent_id))
+		elif sc.TransactionType.MOSAIC_DEFINITION == transaction.type_:
+			address = self.network.public_key_to_address(PublicKey(transaction.signer_public_key.bytes))
+			transaction.id = sc.MosaicId(generate_mosaic_id(address, transaction.nonce.value))
+
+		return transaction
+
+	def create(self, transaction_descriptor, autosort=True):
+		"""
+		Creates a transaction from a transaction descriptor.
+		When autosort is set (default), descriptor arrays requiring ordering will be automatically sorted.
+		When unset, descriptor arrays will be presumed to be already sorted.
+		"""
+		return self._create_and_extend(transaction_descriptor, autosort, sc.TransactionFactory)
+
+	def create_embedded(self, transaction_descriptor, autosort=True):
+		"""
+		Creates an embedded transaction from a transaction descriptor.
+		When autosort is set (default), descriptor arrays requiring ordering will be automatically sorted.
+		When unset, descriptor arrays will be presumed to be already sorted.
+		"""
+		return self._create_and_extend(transaction_descriptor, autosort, sc.EmbeddedTransactionFactory)
 
-	# NOTE: currently `TypeParserBuilder.create_sdk_wrapper`` assumes SDK types are used as keys (although could be `sc` types as well)
-	# resulting sdk type will be converted further via `symbol_type_converter`
 	@staticmethod
-	def _create_symbol_type_to_property_mapping():
-		return {
-			Address: 'address',
-			PublicKey: 'public_key',
-		}
-
-	def hash_transaction(self, transaction):
-		"""Hashes a Symbol transaction."""
-		hasher = sha3.sha3_256()
-		hasher.update(transaction.signature.bytes)
-		hasher.update(transaction.signer_public_key.bytes)
-		hasher.update(self.network.generation_hash_seed.bytes)
-		hasher.update(self._transaction_data_buffer(transaction.serialize()))
-		return Hash256(hasher.digest())
-
-	def sign_transaction(self, key_pair, transaction):
-		"""Signs a Symbol transaction."""
-		sign_buffer = self.network.generation_hash_seed.bytes
-		sign_buffer += self._transaction_data_buffer(transaction.serialize())
-		return key_pair.sign(sign_buffer)
-
-	def verify_transaction(self, transaction, signature):
-		"""Verifies a Symbol transaction."""
-		verify_buffer = self.network.generation_hash_seed.bytes
-		verify_buffer += self._transaction_data_buffer(transaction.serialize())
-		return Verifier(transaction.signer_public_key).verify(verify_buffer, signature)
+	def attach_signature(transaction, signature):
+		"""Attaches a signature to a transaction."""
+		transaction.signature = sc.Signature(signature.bytes)
+
+		transaction_buffer = transaction.serialize()
+		hex_payload = hexlify(transaction_buffer).decode('utf8').upper()
+		json_payload = f'{{"payload": "{hex_payload}"}}'
+		return json_payload
 
 	@staticmethod
-	def hash_embedded_transactions(embedded_transactions):
-		"""Hashes embedded transactions of an aggregate."""
-		hash_builder = MerkleHashBuilder()
-		for embedded_transaction in embedded_transactions:
-			hash_builder.update(Hash256(sha3.sha3_256(embedded_transaction.serialize()).digest()))
-
-		return hash_builder.final()
+	def _symbol_type_converter(value):
+		if isinstance(value, Address):
+			return sc.UnresolvedAddress(value.bytes)
 
-	@staticmethod
-	def bip32_node_to_key_pair(bip32_node):
-		"""Derives a Symbol KeyPair from a BIP32 node."""
-		return KeyPair(bip32_node.private_key)
+		return None
 
 	@staticmethod
-	def _is_aggregate_transaction(transaction_buffer):
-		transaction_type_offset = TRANSACTION_HEADER_SIZE + 2  # skip version and network byte
-		transaction_type = (transaction_buffer[transaction_type_offset + 1] << 8) + transaction_buffer[transaction_type_offset]
-		aggregate_types = [TransactionType.AGGREGATE_BONDED.value, TransactionType.AGGREGATE_COMPLETE.value]
-		return transaction_type in aggregate_types
+	def _build_rules(type_rule_overrides):
+		factory = RuleBasedTransactionFactory(sc, TransactionFactory._symbol_type_converter, type_rule_overrides)
+		factory.autodetect()
+
+		factory.add_struct_parser('UnresolvedMosaic')
+
+		sdk_type_mapping = {
+			'UnresolvedAddress': Address,
+			'Address': Address,
+			'Hash256': Hash256,
+			'PublicKey': PublicKey,
+			'VotingPublicKey': PublicKey,
+		}
+		for name, typename in sdk_type_mapping.items():
+			factory.add_pod_parser(name, typename)
 
-	@staticmethod
-	def _transaction_data_buffer(transaction_buffer):
-		data_buffer_start = TRANSACTION_HEADER_SIZE
-		data_buffer_end = len(transaction_buffer)
-		if SymbolFacade._is_aggregate_transaction(transaction_buffer):
-			data_buffer_end = TRANSACTION_HEADER_SIZE + AGGREGATE_HASHED_SIZE
+		for name in ['UnresolvedMosaicId', 'TransactionType', 'UnresolvedAddress', 'struct:UnresolvedMosaic']:
+			factory.add_array_parser(name)
 
-		return transaction_buffer[data_buffer_start:data_buffer_end]
+		return factory
```

### Comparing `symbol-sdk-python-3.0.3/symbolchain/nc/__init__.py` & `symbol-sdk-python-3.0.5/symbolchain/nc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python
 #
 # Code generated by catbuffer python generator; DO NOT EDIT.
 #
 # pylint: disable=line-too-long, invalid-name, redefined-builtin
 # pylint: disable=too-many-lines, too-many-instance-attributes, too-many-locals, too-many-statements, too-many-public-methods
-# pylint: disable=duplicate-code
+# pylint: disable=duplicate-code, superfluous-parens
 
 from __future__ import annotations
 
 from binascii import hexlify
 from enum import Enum, Flag
 from typing import ByteString, List, TypeVar
 
@@ -205,14 +205,17 @@
 		self._signature = Signature()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._signature_size = 64  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -375,14 +378,17 @@
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -524,15 +530,15 @@
 
 	def serialize(self) -> bytes:
 		buffer = bytes()
 		buffer += self.value.to_bytes(4, byteorder='little', signed=False)
 		return buffer
 
 
-class AccountKeyLinkTransaction:
+class AccountKeyLinkTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.ACCOUNT_KEY_LINK
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
@@ -540,29 +546,32 @@
 		'fee': 'pod:Amount',
 		'deadline': 'pod:Timestamp',
 		'link_action': 'enum:LinkAction',
 		'remote_public_key': 'pod:PublicKey'
 	}
 
 	def __init__(self):
-		self._type_ = AccountKeyLinkTransaction.TRANSACTION_TYPE
-		self._version = AccountKeyLinkTransaction.TRANSACTION_VERSION
+		self._type_ = AccountKeyLinkTransactionV1.TRANSACTION_TYPE
+		self._version = AccountKeyLinkTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._signature = Signature()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._link_action = LinkAction.LINK
 		self._remote_public_key = PublicKey()
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._signature_size = 64  # reserved field
 		self._remote_public_key_size = 32  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -655,15 +664,15 @@
 		size += self.deadline.size
 		size += self.link_action.size
 		size += 4
 		size += self.remote_public_key.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> AccountKeyLinkTransaction:
+	def deserialize(cls, payload: ByteString) -> AccountKeyLinkTransactionV1:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
@@ -690,15 +699,15 @@
 		buffer = buffer[link_action.size:]
 		remote_public_key_size = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		assert remote_public_key_size == 32, f'Invalid value of reserved field ({remote_public_key_size})'
 		remote_public_key = PublicKey.deserialize(buffer)
 		buffer = buffer[remote_public_key.size:]
 
-		instance = AccountKeyLinkTransaction()
+		instance = AccountKeyLinkTransactionV1()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._signature = signature
 		instance._fee = fee
@@ -737,42 +746,45 @@
 		result += f'deadline: {self._deadline.__str__()}, '
 		result += f'link_action: {self._link_action.__str__()}, '
 		result += f'remote_public_key: {self._remote_public_key.__str__()}, '
 		result += ')'
 		return result
 
 
-class NonVerifiableAccountKeyLinkTransaction:
+class NonVerifiableAccountKeyLinkTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.ACCOUNT_KEY_LINK
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
 		'fee': 'pod:Amount',
 		'deadline': 'pod:Timestamp',
 		'link_action': 'enum:LinkAction',
 		'remote_public_key': 'pod:PublicKey'
 	}
 
 	def __init__(self):
-		self._type_ = NonVerifiableAccountKeyLinkTransaction.TRANSACTION_TYPE
-		self._version = NonVerifiableAccountKeyLinkTransaction.TRANSACTION_VERSION
+		self._type_ = NonVerifiableAccountKeyLinkTransactionV1.TRANSACTION_TYPE
+		self._version = NonVerifiableAccountKeyLinkTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._link_action = LinkAction.LINK
 		self._remote_public_key = PublicKey()
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._remote_public_key_size = 32  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -855,15 +867,15 @@
 		size += self.deadline.size
 		size += self.link_action.size
 		size += 4
 		size += self.remote_public_key.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> NonVerifiableAccountKeyLinkTransaction:
+	def deserialize(cls, payload: ByteString) -> NonVerifiableAccountKeyLinkTransactionV1:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
@@ -885,15 +897,15 @@
 		buffer = buffer[link_action.size:]
 		remote_public_key_size = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		assert remote_public_key_size == 32, f'Invalid value of reserved field ({remote_public_key_size})'
 		remote_public_key = PublicKey.deserialize(buffer)
 		buffer = buffer[remote_public_key.size:]
 
-		instance = NonVerifiableAccountKeyLinkTransaction()
+		instance = NonVerifiableAccountKeyLinkTransactionV1()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._fee = fee
 		instance._deadline = deadline
@@ -936,14 +948,17 @@
 	TYPE_HINTS = {
 		'name': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._name = bytes()
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def name(self) -> bytes:
 		return self._name
 
 	@name.setter
 	def name(self, value: bytes):
 		self._name = value
@@ -986,14 +1001,17 @@
 		'name': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._namespace_id = NamespaceId()
 		self._name = bytes()
 
+	def sort(self) -> None:
+		self._namespace_id.sort()
+
 	@property
 	def namespace_id(self) -> NamespaceId:
 		return self._namespace_id
 
 	@property
 	def name(self) -> bytes:
 		return self._name
@@ -1050,14 +1068,17 @@
 		'amount': 'pod:Amount'
 	}
 
 	def __init__(self):
 		self._mosaic_id = MosaicId()
 		self._amount = Amount()
 
+	def sort(self) -> None:
+		self._mosaic_id.sort()
+
 	@property
 	def mosaic_id(self) -> MosaicId:
 		return self._mosaic_id
 
 	@property
 	def amount(self) -> Amount:
 		return self._amount
@@ -1113,14 +1134,17 @@
 	TYPE_HINTS = {
 		'mosaic': 'struct:Mosaic'
 	}
 
 	def __init__(self):
 		self._mosaic = Mosaic()
 
+	def sort(self) -> None:
+		self._mosaic.sort()
+
 	@property
 	def mosaic(self) -> Mosaic:
 		return self._mosaic
 
 	@mosaic.setter
 	def mosaic(self, value: Mosaic):
 		self._mosaic = value
@@ -1188,14 +1212,17 @@
 	def __init__(self):
 		self._transfer_fee_type = MosaicTransferFeeType.ABSOLUTE
 		self._recipient_address = Address()
 		self._mosaic_id = MosaicId()
 		self._fee = Amount()
 		self._recipient_address_size = 40  # reserved field
 
+	def sort(self) -> None:
+		self._mosaic_id.sort()
+
 	@property
 	def transfer_fee_type(self) -> MosaicTransferFeeType:
 		return self._transfer_fee_type
 
 	@property
 	def recipient_address(self) -> Address:
 		return self._recipient_address
@@ -1286,14 +1313,17 @@
 		'value': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._name = bytes()
 		self._value = bytes()
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def name(self) -> bytes:
 		return self._name
 
 	@property
 	def value(self) -> bytes:
 		return self._value
@@ -1352,14 +1382,17 @@
 	TYPE_HINTS = {
 		'property_': 'struct:MosaicProperty'
 	}
 
 	def __init__(self):
 		self._property_ = MosaicProperty()
 
+	def sort(self) -> None:
+		self._property_.sort()
+
 	@property
 	def property_(self) -> MosaicProperty:
 		return self._property_
 
 	@property_.setter
 	def property_(self, value: MosaicProperty):
 		self._property_ = value
@@ -1407,18 +1440,22 @@
 	}
 
 	def __init__(self):
 		self._owner_public_key = PublicKey()
 		self._id = MosaicId()
 		self._description = bytes()
 		self._properties = []
-		self._levy_size = 0
-		self._levy = MosaicLevy()
+		self._levy = None
 		self._owner_public_key_size = 32  # reserved field
 
+	def sort(self) -> None:
+		self._id.sort()
+		if 0 != self.levy_size_computed:
+			self._levy.sort()
+
 	@property
 	def owner_public_key(self) -> PublicKey:
 		return self._owner_public_key
 
 	@property
 	def id(self) -> MosaicId:
 		return self._id
@@ -1428,21 +1465,21 @@
 		return self._description
 
 	@property
 	def properties(self) -> List[SizePrefixedMosaicProperty]:
 		return self._properties
 
 	@property
-	def levy_size(self) -> int:
-		return self._levy_size
-
-	@property
 	def levy(self) -> MosaicLevy:
 		return self._levy
 
+	@property
+	def levy_size_computed(self) -> int:
+		return 0 if not self.levy else self.levy.size + 0
+
 	@owner_public_key.setter
 	def owner_public_key(self, value: PublicKey):
 		self._owner_public_key = value
 
 	@id.setter
 	def id(self, value: MosaicId):
 		self._id = value
@@ -1451,18 +1488,14 @@
 	def description(self, value: bytes):
 		self._description = value
 
 	@properties.setter
 	def properties(self, value: List[SizePrefixedMosaicProperty]):
 		self._properties = value
 
-	@levy_size.setter
-	def levy_size(self, value: int):
-		self._levy_size = value
-
 	@levy.setter
 	def levy(self, value: MosaicLevy):
 		self._levy = value
 
 	@property
 	def size(self) -> int:
 		size = 0
@@ -1471,15 +1504,15 @@
 		size += 4
 		size += self.id.size
 		size += 4
 		size += len(self._description)
 		size += 4
 		size += ArrayHelpers.size(self.properties)
 		size += 4
-		if 0 != self.levy_size:
+		if 0 != self.levy_size_computed:
 			size += self.levy.size
 		return size
 
 	@classmethod
 	def deserialize(cls, payload: ByteString) -> MosaicDefinition:
 		buffer = memoryview(payload)
 		owner_public_key_size = int.from_bytes(buffer[:4], byteorder='little', signed=False)
@@ -1508,47 +1541,45 @@
 			buffer = buffer[levy.size:]
 
 		instance = MosaicDefinition()
 		instance._owner_public_key = owner_public_key
 		instance._id = id
 		instance._description = description
 		instance._properties = properties
-		instance._levy_size = levy_size
 		instance._levy = levy
 		return instance
 
 	def serialize(self) -> bytes:
 		buffer = bytes()
 		buffer += self._owner_public_key_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._owner_public_key.serialize()
 		buffer += self.id.size.to_bytes(4, byteorder='little', signed=False)  # id_size
 		buffer += self._id.serialize()
 		buffer += len(self._description).to_bytes(4, byteorder='little', signed=False)  # description_size
 		buffer += self._description
 		buffer += len(self._properties).to_bytes(4, byteorder='little', signed=False)  # properties_count
 		buffer += ArrayHelpers.write_array(self._properties)
-		buffer += self._levy_size.to_bytes(4, byteorder='little', signed=False)
-		if 0 != self.levy_size:
+		buffer += self.levy_size_computed.to_bytes(4, byteorder='little', signed=False)
+		if 0 != self.levy_size_computed:
 			buffer += self._levy.serialize()
 		return buffer
 
 	def __str__(self) -> str:
 		result = '('
 		result += f'owner_public_key: {self._owner_public_key.__str__()}, '
 		result += f'id: {self._id.__str__()}, '
 		result += f'description: {hexlify(self._description).decode("utf8")}, '
 		result += f'properties: {list(map(str, self._properties))}, '
-		result += f'levy_size: 0x{self._levy_size:X}, '
-		if 0 != self.levy_size:
+		if 0 != self.levy_size_computed:
 			result += f'levy: {self._levy.__str__()}, '
 		result += ')'
 		return result
 
 
-class MosaicDefinitionTransaction:
+class MosaicDefinitionTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_DEFINITION
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
@@ -1557,30 +1588,33 @@
 		'deadline': 'pod:Timestamp',
 		'mosaic_definition': 'struct:MosaicDefinition',
 		'rental_fee_sink': 'pod:Address',
 		'rental_fee': 'pod:Amount'
 	}
 
 	def __init__(self):
-		self._type_ = MosaicDefinitionTransaction.TRANSACTION_TYPE
-		self._version = MosaicDefinitionTransaction.TRANSACTION_VERSION
+		self._type_ = MosaicDefinitionTransactionV1.TRANSACTION_TYPE
+		self._version = MosaicDefinitionTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._signature = Signature()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._mosaic_definition = MosaicDefinition()
 		self._rental_fee_sink = Address()
 		self._rental_fee = Amount()
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._signature_size = 64  # reserved field
 		self._rental_fee_sink_size = 40  # reserved field
 
+	def sort(self) -> None:
+		self._mosaic_definition.sort()
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -1683,15 +1717,15 @@
 		size += self.mosaic_definition.size
 		size += 4
 		size += self.rental_fee_sink.size
 		size += self.rental_fee.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> MosaicDefinitionTransaction:
+	def deserialize(cls, payload: ByteString) -> MosaicDefinitionTransactionV1:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
@@ -1723,15 +1757,15 @@
 		buffer = buffer[4:]
 		assert rental_fee_sink_size == 40, f'Invalid value of reserved field ({rental_fee_sink_size})'
 		rental_fee_sink = Address.deserialize(buffer)
 		buffer = buffer[rental_fee_sink.size:]
 		rental_fee = Amount.deserialize(buffer)
 		buffer = buffer[rental_fee.size:]
 
-		instance = MosaicDefinitionTransaction()
+		instance = MosaicDefinitionTransactionV1()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._signature = signature
 		instance._fee = fee
@@ -1774,15 +1808,15 @@
 		result += f'mosaic_definition: {self._mosaic_definition.__str__()}, '
 		result += f'rental_fee_sink: {self._rental_fee_sink.__str__()}, '
 		result += f'rental_fee: {self._rental_fee.__str__()}, '
 		result += ')'
 		return result
 
 
-class NonVerifiableMosaicDefinitionTransaction:
+class NonVerifiableMosaicDefinitionTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_DEFINITION
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
@@ -1790,28 +1824,31 @@
 		'deadline': 'pod:Timestamp',
 		'mosaic_definition': 'struct:MosaicDefinition',
 		'rental_fee_sink': 'pod:Address',
 		'rental_fee': 'pod:Amount'
 	}
 
 	def __init__(self):
-		self._type_ = NonVerifiableMosaicDefinitionTransaction.TRANSACTION_TYPE
-		self._version = NonVerifiableMosaicDefinitionTransaction.TRANSACTION_VERSION
+		self._type_ = NonVerifiableMosaicDefinitionTransactionV1.TRANSACTION_TYPE
+		self._version = NonVerifiableMosaicDefinitionTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._mosaic_definition = MosaicDefinition()
 		self._rental_fee_sink = Address()
 		self._rental_fee = Amount()
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._rental_fee_sink_size = 40  # reserved field
 
+	def sort(self) -> None:
+		self._mosaic_definition.sort()
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -1904,15 +1941,15 @@
 		size += self.mosaic_definition.size
 		size += 4
 		size += self.rental_fee_sink.size
 		size += self.rental_fee.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> NonVerifiableMosaicDefinitionTransaction:
+	def deserialize(cls, payload: ByteString) -> NonVerifiableMosaicDefinitionTransactionV1:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
@@ -1939,15 +1976,15 @@
 		buffer = buffer[4:]
 		assert rental_fee_sink_size == 40, f'Invalid value of reserved field ({rental_fee_sink_size})'
 		rental_fee_sink = Address.deserialize(buffer)
 		buffer = buffer[rental_fee_sink.size:]
 		rental_fee = Amount.deserialize(buffer)
 		buffer = buffer[rental_fee.size:]
 
-		instance = NonVerifiableMosaicDefinitionTransaction()
+		instance = NonVerifiableMosaicDefinitionTransactionV1()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._fee = fee
 		instance._deadline = deadline
@@ -2005,15 +2042,15 @@
 
 	def serialize(self) -> bytes:
 		buffer = bytes()
 		buffer += self.value.to_bytes(4, byteorder='little', signed=False)
 		return buffer
 
 
-class MosaicSupplyChangeTransaction:
+class MosaicSupplyChangeTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_SUPPLY_CHANGE
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
@@ -2022,29 +2059,32 @@
 		'deadline': 'pod:Timestamp',
 		'mosaic_id': 'struct:MosaicId',
 		'action': 'enum:MosaicSupplyChangeAction',
 		'delta': 'pod:Amount'
 	}
 
 	def __init__(self):
-		self._type_ = MosaicSupplyChangeTransaction.TRANSACTION_TYPE
-		self._version = MosaicSupplyChangeTransaction.TRANSACTION_VERSION
+		self._type_ = MosaicSupplyChangeTransactionV1.TRANSACTION_TYPE
+		self._version = MosaicSupplyChangeTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._signature = Signature()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._mosaic_id = MosaicId()
 		self._action = MosaicSupplyChangeAction.INCREASE
 		self._delta = Amount()
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._signature_size = 64  # reserved field
 
+	def sort(self) -> None:
+		self._mosaic_id.sort()
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -2146,15 +2186,15 @@
 		size += 4
 		size += self.mosaic_id.size
 		size += self.action.size
 		size += self.delta.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> MosaicSupplyChangeTransaction:
+	def deserialize(cls, payload: ByteString) -> MosaicSupplyChangeTransactionV1:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
@@ -2183,15 +2223,15 @@
 		mosaic_id = MosaicId.deserialize(buffer[:mosaic_id_size])
 		buffer = buffer[mosaic_id.size:]
 		action = MosaicSupplyChangeAction.deserialize(buffer)
 		buffer = buffer[action.size:]
 		delta = Amount.deserialize(buffer)
 		buffer = buffer[delta.size:]
 
-		instance = MosaicSupplyChangeTransaction()
+		instance = MosaicSupplyChangeTransactionV1()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._signature = signature
 		instance._fee = fee
@@ -2233,15 +2273,15 @@
 		result += f'mosaic_id: {self._mosaic_id.__str__()}, '
 		result += f'action: {self._action.__str__()}, '
 		result += f'delta: {self._delta.__str__()}, '
 		result += ')'
 		return result
 
 
-class NonVerifiableMosaicSupplyChangeTransaction:
+class NonVerifiableMosaicSupplyChangeTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_SUPPLY_CHANGE
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
@@ -2249,27 +2289,30 @@
 		'deadline': 'pod:Timestamp',
 		'mosaic_id': 'struct:MosaicId',
 		'action': 'enum:MosaicSupplyChangeAction',
 		'delta': 'pod:Amount'
 	}
 
 	def __init__(self):
-		self._type_ = NonVerifiableMosaicSupplyChangeTransaction.TRANSACTION_TYPE
-		self._version = NonVerifiableMosaicSupplyChangeTransaction.TRANSACTION_VERSION
+		self._type_ = NonVerifiableMosaicSupplyChangeTransactionV1.TRANSACTION_TYPE
+		self._version = NonVerifiableMosaicSupplyChangeTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._mosaic_id = MosaicId()
 		self._action = MosaicSupplyChangeAction.INCREASE
 		self._delta = Amount()
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 
+	def sort(self) -> None:
+		self._mosaic_id.sort()
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -2361,15 +2404,15 @@
 		size += 4
 		size += self.mosaic_id.size
 		size += self.action.size
 		size += self.delta.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> NonVerifiableMosaicSupplyChangeTransaction:
+	def deserialize(cls, payload: ByteString) -> NonVerifiableMosaicSupplyChangeTransactionV1:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
@@ -2393,15 +2436,15 @@
 		mosaic_id = MosaicId.deserialize(buffer[:mosaic_id_size])
 		buffer = buffer[mosaic_id.size:]
 		action = MosaicSupplyChangeAction.deserialize(buffer)
 		buffer = buffer[action.size:]
 		delta = Amount.deserialize(buffer)
 		buffer = buffer[delta.size:]
 
-		instance = NonVerifiableMosaicSupplyChangeTransaction()
+		instance = NonVerifiableMosaicSupplyChangeTransactionV1()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._fee = fee
 		instance._deadline = deadline
@@ -2469,14 +2512,25 @@
 	}
 
 	def __init__(self):
 		self._modification_type = MultisigAccountModificationType.ADD_COSIGNATORY
 		self._cosignatory_public_key = PublicKey()
 		self._cosignatory_public_key_size = 32  # reserved field
 
+	def comparer(self) -> tuple:
+		from ..Transforms import ripemd_keccak_256  # pylint: disable=import-outside-toplevel
+
+		return (
+			self.modification_type if not isinstance(self.modification_type, Enum) else self.modification_type.value,
+			ripemd_keccak_256(self.cosignatory_public_key.bytes),
+		)
+
+	def sort(self) -> None:
+		pass
+
 	@property
 	def modification_type(self) -> MultisigAccountModificationType:
 		return self._modification_type
 
 	@property
 	def cosignatory_public_key(self) -> PublicKey:
 		return self._cosignatory_public_key
@@ -2532,14 +2586,17 @@
 	TYPE_HINTS = {
 		'modification': 'struct:MultisigAccountModification'
 	}
 
 	def __init__(self):
 		self._modification = MultisigAccountModification()
 
+	def sort(self) -> None:
+		self._modification.sort()
+
 	@property
 	def modification(self) -> MultisigAccountModification:
 		return self._modification
 
 	@modification.setter
 	def modification(self, value: MultisigAccountModification):
 		self._modification = value
@@ -2601,14 +2658,17 @@
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._modifications = []
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._signature_size = 64  # reserved field
 
+	def sort(self) -> None:
+		self._modifications = sorted(self._modifications, key=lambda e: e.modification.comparer() if hasattr(e.modification, 'comparer') else e.modification)
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -2721,15 +2781,15 @@
 		buffer = buffer[signature.size:]
 		fee = Amount.deserialize(buffer)
 		buffer = buffer[fee.size:]
 		deadline = Timestamp.deserialize(buffer)
 		buffer = buffer[deadline.size:]
 		modifications_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
-		modifications = ArrayHelpers.read_array_count(buffer, SizePrefixedMultisigAccountModification, modifications_count)
+		modifications = ArrayHelpers.read_array_count(buffer, SizePrefixedMultisigAccountModification, modifications_count, lambda e: e.modification.comparer() if hasattr(e.modification, 'comparer') else e.modification)
 		buffer = buffer[ArrayHelpers.size(modifications):]
 
 		instance = MultisigAccountModificationTransactionV1()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
@@ -2750,15 +2810,15 @@
 		buffer += self._signer_public_key_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._signer_public_key.serialize()
 		buffer += self._signature_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._signature.serialize()
 		buffer += self._fee.serialize()
 		buffer += self._deadline.serialize()
 		buffer += len(self._modifications).to_bytes(4, byteorder='little', signed=False)  # modifications_count
-		buffer += ArrayHelpers.write_array(self._modifications)
+		buffer += ArrayHelpers.write_array(self._modifications, lambda e: e.modification.comparer() if hasattr(e.modification, 'comparer') else e.modification)
 		return buffer
 
 	def __str__(self) -> str:
 		result = '('
 		result += f'type_: {self._type_.__str__()}, '
 		result += f'version: 0x{self._version:X}, '
 		result += f'network: {self._network.__str__()}, '
@@ -2793,14 +2853,17 @@
 		self._signer_public_key = PublicKey()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._modifications = []
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 
+	def sort(self) -> None:
+		self._modifications = sorted(self._modifications, key=lambda e: e.modification.comparer() if hasattr(e.modification, 'comparer') else e.modification)
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -2898,15 +2961,15 @@
 		buffer = buffer[signer_public_key.size:]
 		fee = Amount.deserialize(buffer)
 		buffer = buffer[fee.size:]
 		deadline = Timestamp.deserialize(buffer)
 		buffer = buffer[deadline.size:]
 		modifications_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
-		modifications = ArrayHelpers.read_array_count(buffer, SizePrefixedMultisigAccountModification, modifications_count)
+		modifications = ArrayHelpers.read_array_count(buffer, SizePrefixedMultisigAccountModification, modifications_count, lambda e: e.modification.comparer() if hasattr(e.modification, 'comparer') else e.modification)
 		buffer = buffer[ArrayHelpers.size(modifications):]
 
 		instance = NonVerifiableMultisigAccountModificationTransactionV1()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
@@ -2924,15 +2987,15 @@
 		buffer += self._network.serialize()
 		buffer += self._timestamp.serialize()
 		buffer += self._signer_public_key_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._signer_public_key.serialize()
 		buffer += self._fee.serialize()
 		buffer += self._deadline.serialize()
 		buffer += len(self._modifications).to_bytes(4, byteorder='little', signed=False)  # modifications_count
-		buffer += ArrayHelpers.write_array(self._modifications)
+		buffer += ArrayHelpers.write_array(self._modifications, lambda e: e.modification.comparer() if hasattr(e.modification, 'comparer') else e.modification)
 		return buffer
 
 	def __str__(self) -> str:
 		result = '('
 		result += f'type_: {self._type_.__str__()}, '
 		result += f'version: 0x{self._version:X}, '
 		result += f'network: {self._network.__str__()}, '
@@ -2941,44 +3004,47 @@
 		result += f'fee: {self._fee.__str__()}, '
 		result += f'deadline: {self._deadline.__str__()}, '
 		result += f'modifications: {list(map(str, self._modifications))}, '
 		result += ')'
 		return result
 
 
-class MultisigAccountModificationTransaction:
+class MultisigAccountModificationTransactionV2:
 	TRANSACTION_VERSION: int = 2
 	TRANSACTION_TYPE: TransactionType = TransactionType.MULTISIG_ACCOUNT_MODIFICATION
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
 		'signature': 'pod:Signature',
 		'fee': 'pod:Amount',
 		'deadline': 'pod:Timestamp',
 		'modifications': 'array[SizePrefixedMultisigAccountModification]'
 	}
 
 	def __init__(self):
-		self._type_ = MultisigAccountModificationTransaction.TRANSACTION_TYPE
-		self._version = MultisigAccountModificationTransaction.TRANSACTION_VERSION
+		self._type_ = MultisigAccountModificationTransactionV2.TRANSACTION_TYPE
+		self._version = MultisigAccountModificationTransactionV2.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._signature = Signature()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._modifications = []
 		self._min_approval_delta = 0
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._signature_size = 64  # reserved field
 		self._min_approval_delta_size = 4  # reserved field
 
+	def sort(self) -> None:
+		self._modifications = sorted(self._modifications, key=lambda e: e.modification.comparer() if hasattr(e.modification, 'comparer') else e.modification)
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -3072,15 +3138,15 @@
 		size += 4
 		size += ArrayHelpers.size(self.modifications)
 		size += 4
 		size += 4
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> MultisigAccountModificationTransaction:
+	def deserialize(cls, payload: ByteString) -> MultisigAccountModificationTransactionV2:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
@@ -3101,23 +3167,23 @@
 		buffer = buffer[signature.size:]
 		fee = Amount.deserialize(buffer)
 		buffer = buffer[fee.size:]
 		deadline = Timestamp.deserialize(buffer)
 		buffer = buffer[deadline.size:]
 		modifications_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
-		modifications = ArrayHelpers.read_array_count(buffer, SizePrefixedMultisigAccountModification, modifications_count)
+		modifications = ArrayHelpers.read_array_count(buffer, SizePrefixedMultisigAccountModification, modifications_count, lambda e: e.modification.comparer() if hasattr(e.modification, 'comparer') else e.modification)
 		buffer = buffer[ArrayHelpers.size(modifications):]
 		min_approval_delta_size = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		assert min_approval_delta_size == 4, f'Invalid value of reserved field ({min_approval_delta_size})'
 		min_approval_delta = int.from_bytes(buffer[:4], byteorder='little', signed=True)
 		buffer = buffer[4:]
 
-		instance = MultisigAccountModificationTransaction()
+		instance = MultisigAccountModificationTransactionV2()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._signature = signature
 		instance._fee = fee
@@ -3136,15 +3202,15 @@
 		buffer += self._signer_public_key_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._signer_public_key.serialize()
 		buffer += self._signature_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._signature.serialize()
 		buffer += self._fee.serialize()
 		buffer += self._deadline.serialize()
 		buffer += len(self._modifications).to_bytes(4, byteorder='little', signed=False)  # modifications_count
-		buffer += ArrayHelpers.write_array(self._modifications)
+		buffer += ArrayHelpers.write_array(self._modifications, lambda e: e.modification.comparer() if hasattr(e.modification, 'comparer') else e.modification)
 		buffer += self._min_approval_delta_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._min_approval_delta.to_bytes(4, byteorder='little', signed=True)
 		return buffer
 
 	def __str__(self) -> str:
 		result = '('
 		result += f'type_: {self._type_.__str__()}, '
@@ -3157,41 +3223,44 @@
 		result += f'deadline: {self._deadline.__str__()}, '
 		result += f'modifications: {list(map(str, self._modifications))}, '
 		result += f'min_approval_delta: 0x{self._min_approval_delta:X}, '
 		result += ')'
 		return result
 
 
-class NonVerifiableMultisigAccountModificationTransaction:
+class NonVerifiableMultisigAccountModificationTransactionV2:
 	TRANSACTION_VERSION: int = 2
 	TRANSACTION_TYPE: TransactionType = TransactionType.MULTISIG_ACCOUNT_MODIFICATION
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
 		'fee': 'pod:Amount',
 		'deadline': 'pod:Timestamp',
 		'modifications': 'array[SizePrefixedMultisigAccountModification]'
 	}
 
 	def __init__(self):
-		self._type_ = NonVerifiableMultisigAccountModificationTransaction.TRANSACTION_TYPE
-		self._version = NonVerifiableMultisigAccountModificationTransaction.TRANSACTION_VERSION
+		self._type_ = NonVerifiableMultisigAccountModificationTransactionV2.TRANSACTION_TYPE
+		self._version = NonVerifiableMultisigAccountModificationTransactionV2.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._modifications = []
 		self._min_approval_delta = 0
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._min_approval_delta_size = 4  # reserved field
 
+	def sort(self) -> None:
+		self._modifications = sorted(self._modifications, key=lambda e: e.modification.comparer() if hasattr(e.modification, 'comparer') else e.modification)
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -3275,15 +3344,15 @@
 		size += 4
 		size += ArrayHelpers.size(self.modifications)
 		size += 4
 		size += 4
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> NonVerifiableMultisigAccountModificationTransaction:
+	def deserialize(cls, payload: ByteString) -> NonVerifiableMultisigAccountModificationTransactionV2:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
@@ -3299,23 +3368,23 @@
 		buffer = buffer[signer_public_key.size:]
 		fee = Amount.deserialize(buffer)
 		buffer = buffer[fee.size:]
 		deadline = Timestamp.deserialize(buffer)
 		buffer = buffer[deadline.size:]
 		modifications_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
-		modifications = ArrayHelpers.read_array_count(buffer, SizePrefixedMultisigAccountModification, modifications_count)
+		modifications = ArrayHelpers.read_array_count(buffer, SizePrefixedMultisigAccountModification, modifications_count, lambda e: e.modification.comparer() if hasattr(e.modification, 'comparer') else e.modification)
 		buffer = buffer[ArrayHelpers.size(modifications):]
 		min_approval_delta_size = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		assert min_approval_delta_size == 4, f'Invalid value of reserved field ({min_approval_delta_size})'
 		min_approval_delta = int.from_bytes(buffer[:4], byteorder='little', signed=True)
 		buffer = buffer[4:]
 
-		instance = NonVerifiableMultisigAccountModificationTransaction()
+		instance = NonVerifiableMultisigAccountModificationTransactionV2()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._fee = fee
 		instance._deadline = deadline
@@ -3331,15 +3400,15 @@
 		buffer += self._network.serialize()
 		buffer += self._timestamp.serialize()
 		buffer += self._signer_public_key_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._signer_public_key.serialize()
 		buffer += self._fee.serialize()
 		buffer += self._deadline.serialize()
 		buffer += len(self._modifications).to_bytes(4, byteorder='little', signed=False)  # modifications_count
-		buffer += ArrayHelpers.write_array(self._modifications)
+		buffer += ArrayHelpers.write_array(self._modifications, lambda e: e.modification.comparer() if hasattr(e.modification, 'comparer') else e.modification)
 		buffer += self._min_approval_delta_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._min_approval_delta.to_bytes(4, byteorder='little', signed=True)
 		return buffer
 
 	def __str__(self) -> str:
 		result = '('
 		result += f'type_: {self._type_.__str__()}, '
@@ -3351,15 +3420,15 @@
 		result += f'deadline: {self._deadline.__str__()}, '
 		result += f'modifications: {list(map(str, self._modifications))}, '
 		result += f'min_approval_delta: 0x{self._min_approval_delta:X}, '
 		result += ')'
 		return result
 
 
-class Cosignature:
+class CosignatureV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MULTISIG_COSIGNATURE
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
@@ -3367,16 +3436,16 @@
 		'fee': 'pod:Amount',
 		'deadline': 'pod:Timestamp',
 		'multisig_transaction_hash': 'pod:Hash256',
 		'multisig_account_address': 'pod:Address'
 	}
 
 	def __init__(self):
-		self._type_ = Cosignature.TRANSACTION_TYPE
-		self._version = Cosignature.TRANSACTION_VERSION
+		self._type_ = CosignatureV1.TRANSACTION_TYPE
+		self._version = CosignatureV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._signature = Signature()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._multisig_transaction_hash = Hash256()
@@ -3384,14 +3453,17 @@
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._signature_size = 64  # reserved field
 		self._multisig_transaction_hash_outer_size = 36  # reserved field
 		self._multisig_transaction_hash_size = 32  # reserved field
 		self._multisig_account_address_size = 40  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -3486,15 +3558,15 @@
 		size += 4
 		size += self.multisig_transaction_hash.size
 		size += 4
 		size += self.multisig_account_address.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> Cosignature:
+	def deserialize(cls, payload: ByteString) -> CosignatureV1:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
@@ -3527,15 +3599,15 @@
 		buffer = buffer[multisig_transaction_hash.size:]
 		multisig_account_address_size = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		assert multisig_account_address_size == 40, f'Invalid value of reserved field ({multisig_account_address_size})'
 		multisig_account_address = Address.deserialize(buffer)
 		buffer = buffer[multisig_account_address.size:]
 
-		instance = Cosignature()
+		instance = CosignatureV1()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._signature = signature
 		instance._fee = fee
@@ -3576,47 +3648,50 @@
 		result += f'deadline: {self._deadline.__str__()}, '
 		result += f'multisig_transaction_hash: {self._multisig_transaction_hash.__str__()}, '
 		result += f'multisig_account_address: {self._multisig_account_address.__str__()}, '
 		result += ')'
 		return result
 
 
-class SizePrefixedCosignature:
+class SizePrefixedCosignatureV1:
 	TYPE_HINTS = {
-		'cosignature': 'struct:Cosignature'
+		'cosignature': 'struct:CosignatureV1'
 	}
 
 	def __init__(self):
-		self._cosignature = Cosignature()
+		self._cosignature = CosignatureV1()
+
+	def sort(self) -> None:
+		self._cosignature.sort()
 
 	@property
-	def cosignature(self) -> Cosignature:
+	def cosignature(self) -> CosignatureV1:
 		return self._cosignature
 
 	@cosignature.setter
-	def cosignature(self, value: Cosignature):
+	def cosignature(self, value: CosignatureV1):
 		self._cosignature = value
 
 	@property
 	def size(self) -> int:
 		size = 0
 		size += 4
 		size += self.cosignature.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> SizePrefixedCosignature:
+	def deserialize(cls, payload: ByteString) -> SizePrefixedCosignatureV1:
 		buffer = memoryview(payload)
 		cosignature_size = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		# marking sizeof field
-		cosignature = Cosignature.deserialize(buffer[:cosignature_size])
+		cosignature = CosignatureV1.deserialize(buffer[:cosignature_size])
 		buffer = buffer[cosignature.size:]
 
-		instance = SizePrefixedCosignature()
+		instance = SizePrefixedCosignatureV1()
 		instance._cosignature = cosignature
 		return instance
 
 	def serialize(self) -> bytes:
 		buffer = bytes()
 		buffer += self.cosignature.size.to_bytes(4, byteorder='little', signed=False)  # cosignature_size
 		buffer += self._cosignature.serialize()
@@ -3625,44 +3700,47 @@
 	def __str__(self) -> str:
 		result = '('
 		result += f'cosignature: {self._cosignature.__str__()}, '
 		result += ')'
 		return result
 
 
-class MultisigTransaction:
+class MultisigTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MULTISIG_TRANSACTION
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
 		'signature': 'pod:Signature',
 		'fee': 'pod:Amount',
 		'deadline': 'pod:Timestamp',
 		'inner_transaction': 'struct:NonVerifiableTransaction',
-		'cosignatures': 'array[SizePrefixedCosignature]'
+		'cosignatures': 'array[SizePrefixedCosignatureV1]'
 	}
 
 	def __init__(self):
-		self._type_ = MultisigTransaction.TRANSACTION_TYPE
-		self._version = MultisigTransaction.TRANSACTION_VERSION
+		self._type_ = MultisigTransactionV1.TRANSACTION_TYPE
+		self._version = MultisigTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._signature = Signature()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._inner_transaction = NonVerifiableTransaction()
 		self._cosignatures = []
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._signature_size = 64  # reserved field
 
+	def sort(self) -> None:
+		self._inner_transaction.sort()
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -3692,15 +3770,15 @@
 		return self._deadline
 
 	@property
 	def inner_transaction(self) -> NonVerifiableTransaction:
 		return self._inner_transaction
 
 	@property
-	def cosignatures(self) -> List[SizePrefixedCosignature]:
+	def cosignatures(self) -> List[SizePrefixedCosignatureV1]:
 		return self._cosignatures
 
 	@type_.setter
 	def type_(self, value: TransactionType):
 		self._type_ = value
 
 	@version.setter
@@ -3732,15 +3810,15 @@
 		self._deadline = value
 
 	@inner_transaction.setter
 	def inner_transaction(self, value: NonVerifiableTransaction):
 		self._inner_transaction = value
 
 	@cosignatures.setter
-	def cosignatures(self, value: List[SizePrefixedCosignature]):
+	def cosignatures(self, value: List[SizePrefixedCosignatureV1]):
 		self._cosignatures = value
 
 	@property
 	def size(self) -> int:
 		size = 0
 		size += self.type_.size
 		size += 1
@@ -3756,15 +3834,15 @@
 		size += 4
 		size += self.inner_transaction.size
 		size += 4
 		size += ArrayHelpers.size(self.cosignatures)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> MultisigTransaction:
+	def deserialize(cls, payload: ByteString) -> MultisigTransactionV1:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
@@ -3790,18 +3868,18 @@
 		inner_transaction_size = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		# marking sizeof field
 		inner_transaction = NonVerifiableTransactionFactory.deserialize(buffer[:inner_transaction_size])
 		buffer = buffer[inner_transaction.size:]
 		cosignatures_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
-		cosignatures = ArrayHelpers.read_array_count(buffer, SizePrefixedCosignature, cosignatures_count)
+		cosignatures = ArrayHelpers.read_array_count(buffer, SizePrefixedCosignatureV1, cosignatures_count)
 		buffer = buffer[ArrayHelpers.size(cosignatures):]
 
-		instance = MultisigTransaction()
+		instance = MultisigTransactionV1()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._signature = signature
 		instance._fee = fee
@@ -3841,15 +3919,192 @@
 		result += f'deadline: {self._deadline.__str__()}, '
 		result += f'inner_transaction: {self._inner_transaction.__str__()}, '
 		result += f'cosignatures: {list(map(str, self._cosignatures))}, '
 		result += ')'
 		return result
 
 
-class NamespaceRegistrationTransaction:
+class NonVerifiableMultisigTransactionV1:
+	TRANSACTION_VERSION: int = 1
+	TRANSACTION_TYPE: TransactionType = TransactionType.MULTISIG_TRANSACTION
+	TYPE_HINTS = {
+		'type_': 'enum:TransactionType',
+		'network': 'enum:NetworkType',
+		'timestamp': 'pod:Timestamp',
+		'signer_public_key': 'pod:PublicKey',
+		'fee': 'pod:Amount',
+		'deadline': 'pod:Timestamp',
+		'inner_transaction': 'struct:NonVerifiableTransaction'
+	}
+
+	def __init__(self):
+		self._type_ = NonVerifiableMultisigTransactionV1.TRANSACTION_TYPE
+		self._version = NonVerifiableMultisigTransactionV1.TRANSACTION_VERSION
+		self._network = NetworkType.MAINNET
+		self._timestamp = Timestamp()
+		self._signer_public_key = PublicKey()
+		self._fee = Amount()
+		self._deadline = Timestamp()
+		self._inner_transaction = NonVerifiableTransaction()
+		self._entity_body_reserved_1 = 0  # reserved field
+		self._signer_public_key_size = 32  # reserved field
+
+	def sort(self) -> None:
+		self._inner_transaction.sort()
+
+	@property
+	def type_(self) -> TransactionType:
+		return self._type_
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def network(self) -> NetworkType:
+		return self._network
+
+	@property
+	def timestamp(self) -> Timestamp:
+		return self._timestamp
+
+	@property
+	def signer_public_key(self) -> PublicKey:
+		return self._signer_public_key
+
+	@property
+	def fee(self) -> Amount:
+		return self._fee
+
+	@property
+	def deadline(self) -> Timestamp:
+		return self._deadline
+
+	@property
+	def inner_transaction(self) -> NonVerifiableTransaction:
+		return self._inner_transaction
+
+	@type_.setter
+	def type_(self, value: TransactionType):
+		self._type_ = value
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@network.setter
+	def network(self, value: NetworkType):
+		self._network = value
+
+	@timestamp.setter
+	def timestamp(self, value: Timestamp):
+		self._timestamp = value
+
+	@signer_public_key.setter
+	def signer_public_key(self, value: PublicKey):
+		self._signer_public_key = value
+
+	@fee.setter
+	def fee(self, value: Amount):
+		self._fee = value
+
+	@deadline.setter
+	def deadline(self, value: Timestamp):
+		self._deadline = value
+
+	@inner_transaction.setter
+	def inner_transaction(self, value: NonVerifiableTransaction):
+		self._inner_transaction = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += self.type_.size
+		size += 1
+		size += 2
+		size += self.network.size
+		size += self.timestamp.size
+		size += 4
+		size += self.signer_public_key.size
+		size += self.fee.size
+		size += self.deadline.size
+		size += 4
+		size += self.inner_transaction.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> NonVerifiableMultisigTransactionV1:
+		buffer = memoryview(payload)
+		type_ = TransactionType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
+		buffer = buffer[1:]
+		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		assert entity_body_reserved_1 == 0, f'Invalid value of reserved field ({entity_body_reserved_1})'
+		network = NetworkType.deserialize(buffer)
+		buffer = buffer[network.size:]
+		timestamp = Timestamp.deserialize(buffer)
+		buffer = buffer[timestamp.size:]
+		signer_public_key_size = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert signer_public_key_size == 32, f'Invalid value of reserved field ({signer_public_key_size})'
+		signer_public_key = PublicKey.deserialize(buffer)
+		buffer = buffer[signer_public_key.size:]
+		fee = Amount.deserialize(buffer)
+		buffer = buffer[fee.size:]
+		deadline = Timestamp.deserialize(buffer)
+		buffer = buffer[deadline.size:]
+		inner_transaction_size = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		# marking sizeof field
+		inner_transaction = NonVerifiableTransactionFactory.deserialize(buffer[:inner_transaction_size])
+		buffer = buffer[inner_transaction.size:]
+
+		instance = NonVerifiableMultisigTransactionV1()
+		instance._type_ = type_
+		instance._version = version
+		instance._network = network
+		instance._timestamp = timestamp
+		instance._signer_public_key = signer_public_key
+		instance._fee = fee
+		instance._deadline = deadline
+		instance._inner_transaction = inner_transaction
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self._type_.serialize()
+		buffer += self._version.to_bytes(1, byteorder='little', signed=False)
+		buffer += self._entity_body_reserved_1.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._network.serialize()
+		buffer += self._timestamp.serialize()
+		buffer += self._signer_public_key_size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._signer_public_key.serialize()
+		buffer += self._fee.serialize()
+		buffer += self._deadline.serialize()
+		buffer += self.inner_transaction.size.to_bytes(4, byteorder='little', signed=False)  # inner_transaction_size
+		buffer += self._inner_transaction.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'version: 0x{self._version:X}, '
+		result += f'network: {self._network.__str__()}, '
+		result += f'timestamp: {self._timestamp.__str__()}, '
+		result += f'signer_public_key: {self._signer_public_key.__str__()}, '
+		result += f'fee: {self._fee.__str__()}, '
+		result += f'deadline: {self._deadline.__str__()}, '
+		result += f'inner_transaction: {self._inner_transaction.__str__()}, '
+		result += ')'
+		return result
+
+
+class NamespaceRegistrationTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.NAMESPACE_REGISTRATION
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
@@ -3859,31 +4114,34 @@
 		'rental_fee_sink': 'pod:Address',
 		'rental_fee': 'pod:Amount',
 		'name': 'bytes_array',
 		'parent_name': 'bytes_array'
 	}
 
 	def __init__(self):
-		self._type_ = NamespaceRegistrationTransaction.TRANSACTION_TYPE
-		self._version = NamespaceRegistrationTransaction.TRANSACTION_VERSION
+		self._type_ = NamespaceRegistrationTransactionV1.TRANSACTION_TYPE
+		self._version = NamespaceRegistrationTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._signature = Signature()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._rental_fee_sink = Address()
 		self._rental_fee = Amount()
 		self._name = bytes()
-		self._parent_name = bytes()
+		self._parent_name = None
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._signature_size = 64  # reserved field
 		self._rental_fee_sink_size = 40  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -3997,15 +4255,15 @@
 		size += len(self._name)
 		size += 4
 		if self.parent_name:
 			size += len(self._parent_name)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> NamespaceRegistrationTransaction:
+	def deserialize(cls, payload: ByteString) -> NamespaceRegistrationTransactionV1:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
@@ -4042,15 +4300,15 @@
 		parent_name_size = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		parent_name = None
 		if 4294967295 != parent_name_size:
 			parent_name = ArrayHelpers.get_bytes(buffer, parent_name_size)
 			buffer = buffer[parent_name_size:]
 
-		instance = NamespaceRegistrationTransaction()
+		instance = NamespaceRegistrationTransactionV1()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._signature = signature
 		instance._fee = fee
@@ -4099,15 +4357,15 @@
 		result += f'name: {hexlify(self._name).decode("utf8")}, '
 		if self.parent_name:
 			result += f'parent_name: {hexlify(self._parent_name).decode("utf8")}, '
 		result += ')'
 		return result
 
 
-class NonVerifiableNamespaceRegistrationTransaction:
+class NonVerifiableNamespaceRegistrationTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.NAMESPACE_REGISTRATION
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
@@ -4116,29 +4374,32 @@
 		'rental_fee_sink': 'pod:Address',
 		'rental_fee': 'pod:Amount',
 		'name': 'bytes_array',
 		'parent_name': 'bytes_array'
 	}
 
 	def __init__(self):
-		self._type_ = NonVerifiableNamespaceRegistrationTransaction.TRANSACTION_TYPE
-		self._version = NonVerifiableNamespaceRegistrationTransaction.TRANSACTION_VERSION
+		self._type_ = NonVerifiableNamespaceRegistrationTransactionV1.TRANSACTION_TYPE
+		self._version = NonVerifiableNamespaceRegistrationTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._rental_fee_sink = Address()
 		self._rental_fee = Amount()
 		self._name = bytes()
-		self._parent_name = bytes()
+		self._parent_name = None
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._rental_fee_sink_size = 40  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -4242,15 +4503,15 @@
 		size += len(self._name)
 		size += 4
 		if self.parent_name:
 			size += len(self._parent_name)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> NonVerifiableNamespaceRegistrationTransaction:
+	def deserialize(cls, payload: ByteString) -> NonVerifiableNamespaceRegistrationTransactionV1:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
@@ -4282,15 +4543,15 @@
 		parent_name_size = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		parent_name = None
 		if 4294967295 != parent_name_size:
 			parent_name = ArrayHelpers.get_bytes(buffer, parent_name_size)
 			buffer = buffer[parent_name_size:]
 
-		instance = NonVerifiableNamespaceRegistrationTransaction()
+		instance = NonVerifiableNamespaceRegistrationTransactionV1()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._fee = fee
 		instance._deadline = deadline
@@ -4364,14 +4625,17 @@
 		'message': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._message_type = MessageType.PLAIN
 		self._message = bytes()
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def message_type(self) -> MessageType:
 		return self._message_type
 
 	@property
 	def message(self) -> bytes:
 		return self._message
@@ -4445,21 +4709,24 @@
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._signature = Signature()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._recipient_address = Address()
 		self._amount = Amount()
-		self._message_envelope_size = 0
-		self._message = Message()
+		self._message = None
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._signature_size = 64  # reserved field
 		self._recipient_address_size = 40  # reserved field
 
+	def sort(self) -> None:
+		if 0 != self.message_envelope_size_computed:
+			self._message.sort()
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -4493,21 +4760,21 @@
 		return self._recipient_address
 
 	@property
 	def amount(self) -> Amount:
 		return self._amount
 
 	@property
-	def message_envelope_size(self) -> int:
-		return self._message_envelope_size
-
-	@property
 	def message(self) -> Message:
 		return self._message
 
+	@property
+	def message_envelope_size_computed(self) -> int:
+		return 0 if not self.message else self.message.size + 0
+
 	@type_.setter
 	def type_(self, value: TransactionType):
 		self._type_ = value
 
 	@version.setter
 	def version(self, value: int):
 		self._version = value
@@ -4540,18 +4807,14 @@
 	def recipient_address(self, value: Address):
 		self._recipient_address = value
 
 	@amount.setter
 	def amount(self, value: Amount):
 		self._amount = value
 
-	@message_envelope_size.setter
-	def message_envelope_size(self, value: int):
-		self._message_envelope_size = value
-
 	@message.setter
 	def message(self, value: Message):
 		self._message = value
 
 	@property
 	def size(self) -> int:
 		size = 0
@@ -4566,15 +4829,15 @@
 		size += self.signature.size
 		size += self.fee.size
 		size += self.deadline.size
 		size += 4
 		size += self.recipient_address.size
 		size += self.amount.size
 		size += 4
-		if 0 != self.message_envelope_size:
+		if 0 != self.message_envelope_size_computed:
 			size += self.message.size
 		return size
 
 	@classmethod
 	def deserialize(cls, payload: ByteString) -> TransferTransactionV1:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
@@ -4623,15 +4886,14 @@
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._signature = signature
 		instance._fee = fee
 		instance._deadline = deadline
 		instance._recipient_address = recipient_address
 		instance._amount = amount
-		instance._message_envelope_size = message_envelope_size
 		instance._message = message
 		return instance
 
 	def serialize(self) -> bytes:
 		buffer = bytes()
 		buffer += self._type_.serialize()
 		buffer += self._version.to_bytes(1, byteorder='little', signed=False)
@@ -4643,16 +4905,16 @@
 		buffer += self._signature_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._signature.serialize()
 		buffer += self._fee.serialize()
 		buffer += self._deadline.serialize()
 		buffer += self._recipient_address_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._recipient_address.serialize()
 		buffer += self._amount.serialize()
-		buffer += self._message_envelope_size.to_bytes(4, byteorder='little', signed=False)
-		if 0 != self.message_envelope_size:
+		buffer += self.message_envelope_size_computed.to_bytes(4, byteorder='little', signed=False)
+		if 0 != self.message_envelope_size_computed:
 			buffer += self._message.serialize()
 		return buffer
 
 	def __str__(self) -> str:
 		result = '('
 		result += f'type_: {self._type_.__str__()}, '
 		result += f'version: 0x{self._version:X}, '
@@ -4660,16 +4922,15 @@
 		result += f'timestamp: {self._timestamp.__str__()}, '
 		result += f'signer_public_key: {self._signer_public_key.__str__()}, '
 		result += f'signature: {self._signature.__str__()}, '
 		result += f'fee: {self._fee.__str__()}, '
 		result += f'deadline: {self._deadline.__str__()}, '
 		result += f'recipient_address: {self._recipient_address.__str__()}, '
 		result += f'amount: {self._amount.__str__()}, '
-		result += f'message_envelope_size: 0x{self._message_envelope_size:X}, '
-		if 0 != self.message_envelope_size:
+		if 0 != self.message_envelope_size_computed:
 			result += f'message: {self._message.__str__()}, '
 		result += ')'
 		return result
 
 
 class NonVerifiableTransferTransactionV1:
 	TRANSACTION_VERSION: int = 1
@@ -4692,20 +4953,23 @@
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._recipient_address = Address()
 		self._amount = Amount()
-		self._message_envelope_size = 0
-		self._message = Message()
+		self._message = None
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._recipient_address_size = 40  # reserved field
 
+	def sort(self) -> None:
+		if 0 != self.message_envelope_size_computed:
+			self._message.sort()
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -4735,21 +4999,21 @@
 		return self._recipient_address
 
 	@property
 	def amount(self) -> Amount:
 		return self._amount
 
 	@property
-	def message_envelope_size(self) -> int:
-		return self._message_envelope_size
-
-	@property
 	def message(self) -> Message:
 		return self._message
 
+	@property
+	def message_envelope_size_computed(self) -> int:
+		return 0 if not self.message else self.message.size + 0
+
 	@type_.setter
 	def type_(self, value: TransactionType):
 		self._type_ = value
 
 	@version.setter
 	def version(self, value: int):
 		self._version = value
@@ -4778,18 +5042,14 @@
 	def recipient_address(self, value: Address):
 		self._recipient_address = value
 
 	@amount.setter
 	def amount(self, value: Amount):
 		self._amount = value
 
-	@message_envelope_size.setter
-	def message_envelope_size(self, value: int):
-		self._message_envelope_size = value
-
 	@message.setter
 	def message(self, value: Message):
 		self._message = value
 
 	@property
 	def size(self) -> int:
 		size = 0
@@ -4802,15 +5062,15 @@
 		size += self.signer_public_key.size
 		size += self.fee.size
 		size += self.deadline.size
 		size += 4
 		size += self.recipient_address.size
 		size += self.amount.size
 		size += 4
-		if 0 != self.message_envelope_size:
+		if 0 != self.message_envelope_size_computed:
 			size += self.message.size
 		return size
 
 	@classmethod
 	def deserialize(cls, payload: ByteString) -> NonVerifiableTransferTransactionV1:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
@@ -4853,15 +5113,14 @@
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._fee = fee
 		instance._deadline = deadline
 		instance._recipient_address = recipient_address
 		instance._amount = amount
-		instance._message_envelope_size = message_envelope_size
 		instance._message = message
 		return instance
 
 	def serialize(self) -> bytes:
 		buffer = bytes()
 		buffer += self._type_.serialize()
 		buffer += self._version.to_bytes(1, byteorder='little', signed=False)
@@ -4871,38 +5130,37 @@
 		buffer += self._signer_public_key_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._signer_public_key.serialize()
 		buffer += self._fee.serialize()
 		buffer += self._deadline.serialize()
 		buffer += self._recipient_address_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._recipient_address.serialize()
 		buffer += self._amount.serialize()
-		buffer += self._message_envelope_size.to_bytes(4, byteorder='little', signed=False)
-		if 0 != self.message_envelope_size:
+		buffer += self.message_envelope_size_computed.to_bytes(4, byteorder='little', signed=False)
+		if 0 != self.message_envelope_size_computed:
 			buffer += self._message.serialize()
 		return buffer
 
 	def __str__(self) -> str:
 		result = '('
 		result += f'type_: {self._type_.__str__()}, '
 		result += f'version: 0x{self._version:X}, '
 		result += f'network: {self._network.__str__()}, '
 		result += f'timestamp: {self._timestamp.__str__()}, '
 		result += f'signer_public_key: {self._signer_public_key.__str__()}, '
 		result += f'fee: {self._fee.__str__()}, '
 		result += f'deadline: {self._deadline.__str__()}, '
 		result += f'recipient_address: {self._recipient_address.__str__()}, '
 		result += f'amount: {self._amount.__str__()}, '
-		result += f'message_envelope_size: 0x{self._message_envelope_size:X}, '
-		if 0 != self.message_envelope_size:
+		if 0 != self.message_envelope_size_computed:
 			result += f'message: {self._message.__str__()}, '
 		result += ')'
 		return result
 
 
-class TransferTransaction:
+class TransferTransactionV2:
 	TRANSACTION_VERSION: int = 2
 	TRANSACTION_TYPE: TransactionType = TransactionType.TRANSFER
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
@@ -4912,32 +5170,35 @@
 		'recipient_address': 'pod:Address',
 		'amount': 'pod:Amount',
 		'message': 'struct:Message',
 		'mosaics': 'array[SizePrefixedMosaic]'
 	}
 
 	def __init__(self):
-		self._type_ = TransferTransaction.TRANSACTION_TYPE
-		self._version = TransferTransaction.TRANSACTION_VERSION
+		self._type_ = TransferTransactionV2.TRANSACTION_TYPE
+		self._version = TransferTransactionV2.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._signature = Signature()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._recipient_address = Address()
 		self._amount = Amount()
-		self._message_envelope_size = 0
-		self._message = Message()
+		self._message = None
 		self._mosaics = []
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._signature_size = 64  # reserved field
 		self._recipient_address_size = 40  # reserved field
 
+	def sort(self) -> None:
+		if 0 != self.message_envelope_size_computed:
+			self._message.sort()
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -4971,25 +5232,25 @@
 		return self._recipient_address
 
 	@property
 	def amount(self) -> Amount:
 		return self._amount
 
 	@property
-	def message_envelope_size(self) -> int:
-		return self._message_envelope_size
-
-	@property
 	def message(self) -> Message:
 		return self._message
 
 	@property
 	def mosaics(self) -> List[SizePrefixedMosaic]:
 		return self._mosaics
 
+	@property
+	def message_envelope_size_computed(self) -> int:
+		return 0 if not self.message else self.message.size + 0
+
 	@type_.setter
 	def type_(self, value: TransactionType):
 		self._type_ = value
 
 	@version.setter
 	def version(self, value: int):
 		self._version = value
@@ -5022,18 +5283,14 @@
 	def recipient_address(self, value: Address):
 		self._recipient_address = value
 
 	@amount.setter
 	def amount(self, value: Amount):
 		self._amount = value
 
-	@message_envelope_size.setter
-	def message_envelope_size(self, value: int):
-		self._message_envelope_size = value
-
 	@message.setter
 	def message(self, value: Message):
 		self._message = value
 
 	@mosaics.setter
 	def mosaics(self, value: List[SizePrefixedMosaic]):
 		self._mosaics = value
@@ -5052,22 +5309,22 @@
 		size += self.signature.size
 		size += self.fee.size
 		size += self.deadline.size
 		size += 4
 		size += self.recipient_address.size
 		size += self.amount.size
 		size += 4
-		if 0 != self.message_envelope_size:
+		if 0 != self.message_envelope_size_computed:
 			size += self.message.size
 		size += 4
 		size += ArrayHelpers.size(self.mosaics)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> TransferTransaction:
+	def deserialize(cls, payload: ByteString) -> TransferTransactionV2:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
@@ -5104,26 +5361,25 @@
 			message = Message.deserialize(buffer)
 			buffer = buffer[message.size:]
 		mosaics_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		mosaics = ArrayHelpers.read_array_count(buffer, SizePrefixedMosaic, mosaics_count)
 		buffer = buffer[ArrayHelpers.size(mosaics):]
 
-		instance = TransferTransaction()
+		instance = TransferTransactionV2()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._signature = signature
 		instance._fee = fee
 		instance._deadline = deadline
 		instance._recipient_address = recipient_address
 		instance._amount = amount
-		instance._message_envelope_size = message_envelope_size
 		instance._message = message
 		instance._mosaics = mosaics
 		return instance
 
 	def serialize(self) -> bytes:
 		buffer = bytes()
 		buffer += self._type_.serialize()
@@ -5136,16 +5392,16 @@
 		buffer += self._signature_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._signature.serialize()
 		buffer += self._fee.serialize()
 		buffer += self._deadline.serialize()
 		buffer += self._recipient_address_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._recipient_address.serialize()
 		buffer += self._amount.serialize()
-		buffer += self._message_envelope_size.to_bytes(4, byteorder='little', signed=False)
-		if 0 != self.message_envelope_size:
+		buffer += self.message_envelope_size_computed.to_bytes(4, byteorder='little', signed=False)
+		if 0 != self.message_envelope_size_computed:
 			buffer += self._message.serialize()
 		buffer += len(self._mosaics).to_bytes(4, byteorder='little', signed=False)  # mosaics_count
 		buffer += ArrayHelpers.write_array(self._mosaics)
 		return buffer
 
 	def __str__(self) -> str:
 		result = '('
@@ -5155,23 +5411,22 @@
 		result += f'timestamp: {self._timestamp.__str__()}, '
 		result += f'signer_public_key: {self._signer_public_key.__str__()}, '
 		result += f'signature: {self._signature.__str__()}, '
 		result += f'fee: {self._fee.__str__()}, '
 		result += f'deadline: {self._deadline.__str__()}, '
 		result += f'recipient_address: {self._recipient_address.__str__()}, '
 		result += f'amount: {self._amount.__str__()}, '
-		result += f'message_envelope_size: 0x{self._message_envelope_size:X}, '
-		if 0 != self.message_envelope_size:
+		if 0 != self.message_envelope_size_computed:
 			result += f'message: {self._message.__str__()}, '
 		result += f'mosaics: {list(map(str, self._mosaics))}, '
 		result += ')'
 		return result
 
 
-class NonVerifiableTransferTransaction:
+class NonVerifiableTransferTransactionV2:
 	TRANSACTION_VERSION: int = 2
 	TRANSACTION_TYPE: TransactionType = TransactionType.TRANSFER
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
@@ -5180,30 +5435,33 @@
 		'recipient_address': 'pod:Address',
 		'amount': 'pod:Amount',
 		'message': 'struct:Message',
 		'mosaics': 'array[SizePrefixedMosaic]'
 	}
 
 	def __init__(self):
-		self._type_ = NonVerifiableTransferTransaction.TRANSACTION_TYPE
-		self._version = NonVerifiableTransferTransaction.TRANSACTION_VERSION
+		self._type_ = NonVerifiableTransferTransactionV2.TRANSACTION_TYPE
+		self._version = NonVerifiableTransferTransactionV2.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
 		self._timestamp = Timestamp()
 		self._signer_public_key = PublicKey()
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._recipient_address = Address()
 		self._amount = Amount()
-		self._message_envelope_size = 0
-		self._message = Message()
+		self._message = None
 		self._mosaics = []
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._signer_public_key_size = 32  # reserved field
 		self._recipient_address_size = 40  # reserved field
 
+	def sort(self) -> None:
+		if 0 != self.message_envelope_size_computed:
+			self._message.sort()
+
 	@property
 	def type_(self) -> TransactionType:
 		return self._type_
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -5233,25 +5491,25 @@
 		return self._recipient_address
 
 	@property
 	def amount(self) -> Amount:
 		return self._amount
 
 	@property
-	def message_envelope_size(self) -> int:
-		return self._message_envelope_size
-
-	@property
 	def message(self) -> Message:
 		return self._message
 
 	@property
 	def mosaics(self) -> List[SizePrefixedMosaic]:
 		return self._mosaics
 
+	@property
+	def message_envelope_size_computed(self) -> int:
+		return 0 if not self.message else self.message.size + 0
+
 	@type_.setter
 	def type_(self, value: TransactionType):
 		self._type_ = value
 
 	@version.setter
 	def version(self, value: int):
 		self._version = value
@@ -5280,18 +5538,14 @@
 	def recipient_address(self, value: Address):
 		self._recipient_address = value
 
 	@amount.setter
 	def amount(self, value: Amount):
 		self._amount = value
 
-	@message_envelope_size.setter
-	def message_envelope_size(self, value: int):
-		self._message_envelope_size = value
-
 	@message.setter
 	def message(self, value: Message):
 		self._message = value
 
 	@mosaics.setter
 	def mosaics(self, value: List[SizePrefixedMosaic]):
 		self._mosaics = value
@@ -5308,22 +5562,22 @@
 		size += self.signer_public_key.size
 		size += self.fee.size
 		size += self.deadline.size
 		size += 4
 		size += self.recipient_address.size
 		size += self.amount.size
 		size += 4
-		if 0 != self.message_envelope_size:
+		if 0 != self.message_envelope_size_computed:
 			size += self.message.size
 		size += 4
 		size += ArrayHelpers.size(self.mosaics)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> NonVerifiableTransferTransaction:
+	def deserialize(cls, payload: ByteString) -> NonVerifiableTransferTransactionV2:
 		buffer = memoryview(payload)
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		entity_body_reserved_1 = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
@@ -5355,25 +5609,24 @@
 			message = Message.deserialize(buffer)
 			buffer = buffer[message.size:]
 		mosaics_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		mosaics = ArrayHelpers.read_array_count(buffer, SizePrefixedMosaic, mosaics_count)
 		buffer = buffer[ArrayHelpers.size(mosaics):]
 
-		instance = NonVerifiableTransferTransaction()
+		instance = NonVerifiableTransferTransactionV2()
 		instance._type_ = type_
 		instance._version = version
 		instance._network = network
 		instance._timestamp = timestamp
 		instance._signer_public_key = signer_public_key
 		instance._fee = fee
 		instance._deadline = deadline
 		instance._recipient_address = recipient_address
 		instance._amount = amount
-		instance._message_envelope_size = message_envelope_size
 		instance._message = message
 		instance._mosaics = mosaics
 		return instance
 
 	def serialize(self) -> bytes:
 		buffer = bytes()
 		buffer += self._type_.serialize()
@@ -5384,16 +5637,16 @@
 		buffer += self._signer_public_key_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._signer_public_key.serialize()
 		buffer += self._fee.serialize()
 		buffer += self._deadline.serialize()
 		buffer += self._recipient_address_size.to_bytes(4, byteorder='little', signed=False)
 		buffer += self._recipient_address.serialize()
 		buffer += self._amount.serialize()
-		buffer += self._message_envelope_size.to_bytes(4, byteorder='little', signed=False)
-		if 0 != self.message_envelope_size:
+		buffer += self.message_envelope_size_computed.to_bytes(4, byteorder='little', signed=False)
+		if 0 != self.message_envelope_size_computed:
 			buffer += self._message.serialize()
 		buffer += len(self._mosaics).to_bytes(4, byteorder='little', signed=False)  # mosaics_count
 		buffer += ArrayHelpers.write_array(self._mosaics)
 		return buffer
 
 	def __str__(self) -> str:
 		result = '('
@@ -5402,93 +5655,94 @@
 		result += f'network: {self._network.__str__()}, '
 		result += f'timestamp: {self._timestamp.__str__()}, '
 		result += f'signer_public_key: {self._signer_public_key.__str__()}, '
 		result += f'fee: {self._fee.__str__()}, '
 		result += f'deadline: {self._deadline.__str__()}, '
 		result += f'recipient_address: {self._recipient_address.__str__()}, '
 		result += f'amount: {self._amount.__str__()}, '
-		result += f'message_envelope_size: 0x{self._message_envelope_size:X}, '
-		if 0 != self.message_envelope_size:
+		if 0 != self.message_envelope_size_computed:
 			result += f'message: {self._message.__str__()}, '
 		result += f'mosaics: {list(map(str, self._mosaics))}, '
 		result += ')'
 		return result
 
 
 class TransactionFactory:
 	@classmethod
 	def deserialize(cls, payload: bytes) -> Transaction:
 		buffer = bytes(payload)
 		parent = Transaction.deserialize(buffer)
 		mapping = {
-			(AccountKeyLinkTransaction.TRANSACTION_TYPE, AccountKeyLinkTransaction.TRANSACTION_VERSION): AccountKeyLinkTransaction,
-			(MosaicDefinitionTransaction.TRANSACTION_TYPE, MosaicDefinitionTransaction.TRANSACTION_VERSION): MosaicDefinitionTransaction,
-			(MosaicSupplyChangeTransaction.TRANSACTION_TYPE, MosaicSupplyChangeTransaction.TRANSACTION_VERSION): MosaicSupplyChangeTransaction,
+			(AccountKeyLinkTransactionV1.TRANSACTION_TYPE, AccountKeyLinkTransactionV1.TRANSACTION_VERSION): AccountKeyLinkTransactionV1,
+			(MosaicDefinitionTransactionV1.TRANSACTION_TYPE, MosaicDefinitionTransactionV1.TRANSACTION_VERSION): MosaicDefinitionTransactionV1,
+			(MosaicSupplyChangeTransactionV1.TRANSACTION_TYPE, MosaicSupplyChangeTransactionV1.TRANSACTION_VERSION): MosaicSupplyChangeTransactionV1,
 			(MultisigAccountModificationTransactionV1.TRANSACTION_TYPE, MultisigAccountModificationTransactionV1.TRANSACTION_VERSION): MultisigAccountModificationTransactionV1,
-			(MultisigAccountModificationTransaction.TRANSACTION_TYPE, MultisigAccountModificationTransaction.TRANSACTION_VERSION): MultisigAccountModificationTransaction,
-			(Cosignature.TRANSACTION_TYPE, Cosignature.TRANSACTION_VERSION): Cosignature,
-			(MultisigTransaction.TRANSACTION_TYPE, MultisigTransaction.TRANSACTION_VERSION): MultisigTransaction,
-			(NamespaceRegistrationTransaction.TRANSACTION_TYPE, NamespaceRegistrationTransaction.TRANSACTION_VERSION): NamespaceRegistrationTransaction,
+			(MultisigAccountModificationTransactionV2.TRANSACTION_TYPE, MultisigAccountModificationTransactionV2.TRANSACTION_VERSION): MultisigAccountModificationTransactionV2,
+			(CosignatureV1.TRANSACTION_TYPE, CosignatureV1.TRANSACTION_VERSION): CosignatureV1,
+			(MultisigTransactionV1.TRANSACTION_TYPE, MultisigTransactionV1.TRANSACTION_VERSION): MultisigTransactionV1,
+			(NamespaceRegistrationTransactionV1.TRANSACTION_TYPE, NamespaceRegistrationTransactionV1.TRANSACTION_VERSION): NamespaceRegistrationTransactionV1,
 			(TransferTransactionV1.TRANSACTION_TYPE, TransferTransactionV1.TRANSACTION_VERSION): TransferTransactionV1,
-			(TransferTransaction.TRANSACTION_TYPE, TransferTransaction.TRANSACTION_VERSION): TransferTransaction
+			(TransferTransactionV2.TRANSACTION_TYPE, TransferTransactionV2.TRANSACTION_VERSION): TransferTransactionV2
 		}
 		discriminator = (parent.type_, parent.version)
 		factory_class = mapping[discriminator]
 		return factory_class.deserialize(buffer)
 
 	@classmethod
 	def create_by_name(cls, entity_name: str) -> Transaction:
 		mapping = {
-			'account_key_link_transaction': AccountKeyLinkTransaction,
-			'mosaic_definition_transaction': MosaicDefinitionTransaction,
-			'mosaic_supply_change_transaction': MosaicSupplyChangeTransaction,
+			'account_key_link_transaction_v1': AccountKeyLinkTransactionV1,
+			'mosaic_definition_transaction_v1': MosaicDefinitionTransactionV1,
+			'mosaic_supply_change_transaction_v1': MosaicSupplyChangeTransactionV1,
 			'multisig_account_modification_transaction_v1': MultisigAccountModificationTransactionV1,
-			'multisig_account_modification_transaction': MultisigAccountModificationTransaction,
-			'cosignature': Cosignature,
-			'multisig_transaction': MultisigTransaction,
-			'namespace_registration_transaction': NamespaceRegistrationTransaction,
+			'multisig_account_modification_transaction_v2': MultisigAccountModificationTransactionV2,
+			'cosignature_v1': CosignatureV1,
+			'multisig_transaction_v1': MultisigTransactionV1,
+			'namespace_registration_transaction_v1': NamespaceRegistrationTransactionV1,
 			'transfer_transaction_v1': TransferTransactionV1,
-			'transfer_transaction': TransferTransaction
+			'transfer_transaction_v2': TransferTransactionV2
 		}
 
 		if entity_name not in mapping:
-			raise ValueError('unknown Transaction type')
+			raise ValueError(f'unknown Transaction type {entity_name}')
 
 		return mapping[entity_name]()
 
 
 class NonVerifiableTransactionFactory:
 	@classmethod
 	def deserialize(cls, payload: bytes) -> NonVerifiableTransaction:
 		buffer = bytes(payload)
 		parent = NonVerifiableTransaction.deserialize(buffer)
 		mapping = {
-			(NonVerifiableAccountKeyLinkTransaction.TRANSACTION_TYPE, NonVerifiableAccountKeyLinkTransaction.TRANSACTION_VERSION): NonVerifiableAccountKeyLinkTransaction,
-			(NonVerifiableMosaicDefinitionTransaction.TRANSACTION_TYPE, NonVerifiableMosaicDefinitionTransaction.TRANSACTION_VERSION): NonVerifiableMosaicDefinitionTransaction,
-			(NonVerifiableMosaicSupplyChangeTransaction.TRANSACTION_TYPE, NonVerifiableMosaicSupplyChangeTransaction.TRANSACTION_VERSION): NonVerifiableMosaicSupplyChangeTransaction,
+			(NonVerifiableAccountKeyLinkTransactionV1.TRANSACTION_TYPE, NonVerifiableAccountKeyLinkTransactionV1.TRANSACTION_VERSION): NonVerifiableAccountKeyLinkTransactionV1,
+			(NonVerifiableMosaicDefinitionTransactionV1.TRANSACTION_TYPE, NonVerifiableMosaicDefinitionTransactionV1.TRANSACTION_VERSION): NonVerifiableMosaicDefinitionTransactionV1,
+			(NonVerifiableMosaicSupplyChangeTransactionV1.TRANSACTION_TYPE, NonVerifiableMosaicSupplyChangeTransactionV1.TRANSACTION_VERSION): NonVerifiableMosaicSupplyChangeTransactionV1,
 			(NonVerifiableMultisigAccountModificationTransactionV1.TRANSACTION_TYPE, NonVerifiableMultisigAccountModificationTransactionV1.TRANSACTION_VERSION): NonVerifiableMultisigAccountModificationTransactionV1,
-			(NonVerifiableMultisigAccountModificationTransaction.TRANSACTION_TYPE, NonVerifiableMultisigAccountModificationTransaction.TRANSACTION_VERSION): NonVerifiableMultisigAccountModificationTransaction,
-			(NonVerifiableNamespaceRegistrationTransaction.TRANSACTION_TYPE, NonVerifiableNamespaceRegistrationTransaction.TRANSACTION_VERSION): NonVerifiableNamespaceRegistrationTransaction,
+			(NonVerifiableMultisigAccountModificationTransactionV2.TRANSACTION_TYPE, NonVerifiableMultisigAccountModificationTransactionV2.TRANSACTION_VERSION): NonVerifiableMultisigAccountModificationTransactionV2,
+			(NonVerifiableMultisigTransactionV1.TRANSACTION_TYPE, NonVerifiableMultisigTransactionV1.TRANSACTION_VERSION): NonVerifiableMultisigTransactionV1,
+			(NonVerifiableNamespaceRegistrationTransactionV1.TRANSACTION_TYPE, NonVerifiableNamespaceRegistrationTransactionV1.TRANSACTION_VERSION): NonVerifiableNamespaceRegistrationTransactionV1,
 			(NonVerifiableTransferTransactionV1.TRANSACTION_TYPE, NonVerifiableTransferTransactionV1.TRANSACTION_VERSION): NonVerifiableTransferTransactionV1,
-			(NonVerifiableTransferTransaction.TRANSACTION_TYPE, NonVerifiableTransferTransaction.TRANSACTION_VERSION): NonVerifiableTransferTransaction
+			(NonVerifiableTransferTransactionV2.TRANSACTION_TYPE, NonVerifiableTransferTransactionV2.TRANSACTION_VERSION): NonVerifiableTransferTransactionV2
 		}
 		discriminator = (parent.type_, parent.version)
 		factory_class = mapping[discriminator]
 		return factory_class.deserialize(buffer)
 
 	@classmethod
 	def create_by_name(cls, entity_name: str) -> NonVerifiableTransaction:
 		mapping = {
-			'non_verifiable_account_key_link_transaction': NonVerifiableAccountKeyLinkTransaction,
-			'non_verifiable_mosaic_definition_transaction': NonVerifiableMosaicDefinitionTransaction,
-			'non_verifiable_mosaic_supply_change_transaction': NonVerifiableMosaicSupplyChangeTransaction,
+			'non_verifiable_account_key_link_transaction_v1': NonVerifiableAccountKeyLinkTransactionV1,
+			'non_verifiable_mosaic_definition_transaction_v1': NonVerifiableMosaicDefinitionTransactionV1,
+			'non_verifiable_mosaic_supply_change_transaction_v1': NonVerifiableMosaicSupplyChangeTransactionV1,
 			'non_verifiable_multisig_account_modification_transaction_v1': NonVerifiableMultisigAccountModificationTransactionV1,
-			'non_verifiable_multisig_account_modification_transaction': NonVerifiableMultisigAccountModificationTransaction,
-			'non_verifiable_namespace_registration_transaction': NonVerifiableNamespaceRegistrationTransaction,
+			'non_verifiable_multisig_account_modification_transaction_v2': NonVerifiableMultisigAccountModificationTransactionV2,
+			'non_verifiable_multisig_transaction_v1': NonVerifiableMultisigTransactionV1,
+			'non_verifiable_namespace_registration_transaction_v1': NonVerifiableNamespaceRegistrationTransactionV1,
 			'non_verifiable_transfer_transaction_v1': NonVerifiableTransferTransactionV1,
-			'non_verifiable_transfer_transaction': NonVerifiableTransferTransaction
+			'non_verifiable_transfer_transaction_v2': NonVerifiableTransferTransactionV2
 		}
 
 		if entity_name not in mapping:
-			raise ValueError('unknown NonVerifiableTransaction type')
+			raise ValueError(f'unknown NonVerifiableTransaction type {entity_name}')
 
 		return mapping[entity_name]()
```

### Comparing `symbol-sdk-python-3.0.3/symbolchain/nem/KeyPair.py` & `symbol-sdk-python-3.0.5/symbolchain/symbol/KeyPair.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,49 @@
-import sha3
+from cryptography.exceptions import InvalidSignature
+from cryptography.hazmat.primitives import serialization
+from cryptography.hazmat.primitives.asymmetric import ed25519
 
 from ..CryptoTypes import PrivateKey, PublicKey, Signature
-from .external import ed25519
 
 
 class KeyPair:
 	"""Represents an ED25519 private and public key."""
 
 	def __init__(self, private_key):
 		"""Creates a key pair from a private key."""
-		self._sk = private_key.bytes[::-1]
-		self._pk = ed25519.publickey_hash_unsafe(self._sk, sha3.keccak_512)
+		self._sk = ed25519.Ed25519PrivateKey.from_private_bytes(private_key.bytes)
 
 	@property
 	def public_key(self):
 		"""Gets the public key."""
-		return PublicKey(self._pk)
+		return PublicKey(self._sk.public_key().public_bytes(serialization.Encoding.Raw, serialization.PublicFormat.Raw))
 
 	@property
 	def private_key(self):
 		"""Gets the private key."""
-		return PrivateKey(self._sk[::-1])
+		return PrivateKey(self._sk.private_bytes(
+			encoding=serialization.Encoding.Raw,
+			format=serialization.PrivateFormat.Raw,
+			encryption_algorithm=serialization.NoEncryption()))
 
 	def sign(self, message):
 		"""Signs a message with the private key."""
-		return Signature(ed25519.signature_hash_unsafe(message, self._sk, self._pk, sha3.keccak_512))
+		return Signature(self._sk.sign(message))
 
 
 class Verifier:
 	"""Verifies signatures signed by a single key pair."""
 
 	def __init__(self, public_key):
 		"""Creates a verifier from a public key."""
-		self._pk = public_key.bytes
+		if bytes(32) == public_key.bytes:
+			raise ValueError('public key cannot be zero')
+
+		self._pk = ed25519.Ed25519PublicKey.from_public_bytes(public_key.bytes)
 
 	def verify(self, message, signature):
 		"""Verifies a message signature."""
 		try:
-			ed25519.checkvalid_hash(signature.bytes, message, self._pk, sha3.keccak_512)
+			self._pk.verify(signature.bytes, message)
 			return True
-		except (ValueError, ed25519.SignatureMismatch):
+		except InvalidSignature:
 			return False
```

### Comparing `symbol-sdk-python-3.0.3/symbolchain/nem/TransactionFactory.py` & `symbol-sdk-python-3.0.5/symbolchain/nem/TransactionFactory.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,29 @@
 	"""Factory for creating NEM transactions."""
 
 	def __init__(self, network, type_rule_overrides=None):
 		"""Creates a factory for the specified network."""
 		self.factory = self._build_rules(type_rule_overrides)
 		self.network = network
 
-	def create(self, transaction_descriptor):
-		"""Creates a transaction from a transaction descriptor."""
+	def create(self, transaction_descriptor, autosort=True):
+		"""
+		Creates a transaction from a transaction descriptor.
+		When autosort is set (default), descriptor arrays requiring ordering will be automatically sorted.
+		When unset, descriptor arrays will be presumed to be already sorted.
+		"""
 		transaction = self.factory.create_from_factory(nc.TransactionFactory.create_by_name, {
 			**transaction_descriptor,
 			'network': self.network.identifier
 		})
+		if autosort:
+			transaction.sort()
 
 		# hack: explicitly translate transfer message
-		if nc.TransactionType.TRANSFER == transaction.type_ and isinstance(transaction.message.message, str):
+		if nc.TransactionType.TRANSFER == transaction.type_ and transaction.message and isinstance(transaction.message.message, str):
 			transaction.message.message = transaction.message.message.encode('utf8')
 
 		return transaction
 
 	@staticmethod
 	def to_non_verifiable_transaction(transaction):
 		"""Converts a transaction to a non-verifiable transaction."""
@@ -35,15 +41,15 @@
 		if not non_verifiable_class_name.startswith('NonVerifiable'):
 			non_verifiable_class_name = f'NonVerifiable{non_verifiable_class_name}'
 
 		non_verifiable_class = getattr(nc, non_verifiable_class_name)
 		non_verifiable_transaction = non_verifiable_class()
 		for key in dir(non_verifiable_transaction):
 			# isupper() to quickly filter out class properties like TRANSACTION_VERSION or TYPE_HINTS
-			if key.startswith('_') or key[0].isupper() or key in ['size', 'serialize', 'deserialize']:
+			if key.startswith('_') or key[0].isupper() or key in ('size', 'serialize', 'deserialize') or key.endswith('_computed'):
 				continue
 
 			setattr(non_verifiable_transaction, key, getattr(transaction, key))
 
 		return non_verifiable_transaction
 
 	@staticmethod
@@ -66,29 +72,29 @@
 
 	@staticmethod
 	def _build_rules(type_rule_overrides):
 		factory = RuleBasedTransactionFactory(nc, TransactionFactory._nem_type_converter, type_rule_overrides)
 		factory.autodetect()
 
 		struct_names = [
-			'Cosignature', 'Message', 'NamespaceId', 'MosaicId', 'Mosaic', 'SizePrefixedMosaic', 'MosaicLevy',
+			'CosignatureV1', 'Message', 'NamespaceId', 'MosaicId', 'Mosaic', 'SizePrefixedMosaic', 'MosaicLevy',
 			'MosaicProperty', 'SizePrefixedMosaicProperty', 'MosaicDefinition',
-			'MultisigAccountModification', 'SizePrefixedMultisigAccountModification', 'SizePrefixedCosignature'
+			'MultisigAccountModification', 'SizePrefixedMultisigAccountModification', 'SizePrefixedCosignatureV1'
 		]
 		for name in struct_names:
 			factory.add_struct_parser(name)
 
 		sdk_type_mapping = {
 			'Address': Address,
 			'Hash256': Hash256,
 			'PublicKey': PublicKey,
 		}
 		for name, typename in sdk_type_mapping.items():
 			factory.add_pod_parser(name, typename)
 
 		array_names = [
-			'SizePrefixedMosaic', 'SizePrefixedMosaicProperty', 'SizePrefixedMultisigAccountModification', 'SizePrefixedCosignature'
+			'SizePrefixedMosaic', 'SizePrefixedMosaicProperty', 'SizePrefixedMultisigAccountModification', 'SizePrefixedCosignatureV1'
 		]
 		for name in array_names:
 			factory.add_array_parser(f'struct:{name}')
 
 		return factory
```

### Comparing `symbol-sdk-python-3.0.3/symbolchain/nem/external/ed25519.py` & `symbol-sdk-python-3.0.5/symbolchain/external/ed25519.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 or less time to execute an operation depending on the values of the
 inputs, and its memory access patterns may also depend on the inputs.
 This opens it to timing and cache side-channel attacks which can
 disclose data to an attacker.  We rely on Python's long-integer
 arithmetic, so we cannot handle secrets without risking their disclosure.
 """
 
-# pylint: disable=invalid-name,too-many-locals,unused-variable,arguments-out-of-order
+# pylint: disable=invalid-name,too-many-locals,unused-variable,arguments-out-of-order,consider-using-generator
 
 import hashlib
 import operator
 
 __version__ = '1.0.dev0'
 
 
@@ -231,34 +231,63 @@
 		hashobj
 	)
 	R = scalarmult_B(r)
 	S = (r + Hint_hash(encodepoint(R) + pk + m, hashobj) * a) % l_
 	return encodepoint(R) + encodeint(S)
 
 
+def derive_shared_secret_unsafe(pk, sk, hashobj=hashlib.sha512):
+	"""
+	Not safe to use with secret keys or secret data.
+
+	See module docstring.  This function should be used for testing only.
+	"""
+	if not iscanonical(pk):
+		raise ValueError('point is not canonical')
+	A = decodepoint(pk)
+	if not isinmainsubgroup(A):
+		raise ValueError('point is not in main subgroup')
+
+	h = hashobj(sk).digest()
+	a = 2 ** (b - 2) + sum(2 ** i * bit(h, i) for i in range(3, b - 2))
+	P = scalarmult(A, a)
+	return encodepoint(P)
+
+
 def isoncurve(P):
 	(x, y, z, t) = P
 	return z % q != 0 and x * y % q == z * t % q and (y * y - x * x - z * z - d * t * t) % q == 0
 
 
 def decodeint(s):
 	return sum(2 ** i * bit(s, i) for i in range(0, b))
 
 
+def iscanonical(s):
+	"""public key s is canonical if y coordinate is smaller than prime `q`."""
+	return sum(2 ** i * bit(s, i) for i in range(0, b - 1)) < q
+
+
 def decodepoint(s):
 	y = sum(2 ** i * bit(s, i) for i in range(0, b - 1))
 	x = xrecover(y)
 	if x & 1 != bit(s, b - 1):
 		x = q - x
 	P = (x, y, 1, (x * y) % q)
 	if not isoncurve(P):
 		raise ValueError('decoding point that is not on curve')
 	return P
 
 
+def isinmainsubgroup(P):
+	"""checks if point P is in main subgroup."""
+	H = scalarmult(P, l_)
+	return 0 == H[0] and H[1] == H[2]
+
+
 class SignatureMismatch(Exception):
 	pass
 
 
 def checkvalid_hash(s, m, pk, hashobj=hashlib.sha512):
 	"""
 	Not safe to use when any argument is secret.
```

### Comparing `symbol-sdk-python-3.0.3/symbolchain/sc/__init__.py` & `symbol-sdk-python-3.0.5/symbolchain/sc/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python
 #
 # Code generated by catbuffer python generator; DO NOT EDIT.
 #
 # pylint: disable=line-too-long, invalid-name, redefined-builtin
 # pylint: disable=too-many-lines, too-many-instance-attributes, too-many-locals, too-many-statements, too-many-public-methods
-# pylint: disable=duplicate-code
+# pylint: disable=duplicate-code, superfluous-parens
 
 from __future__ import annotations
 
 from binascii import hexlify
 from enum import Enum, Flag
 from typing import ByteString, List, TypeVar
 
@@ -339,14 +339,17 @@
 		'amount': 'pod:Amount'
 	}
 
 	def __init__(self):
 		self._mosaic_id = MosaicId()
 		self._amount = Amount()
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def mosaic_id(self) -> MosaicId:
 		return self._mosaic_id
 
 	@property
 	def amount(self) -> Amount:
 		return self._amount
@@ -399,14 +402,17 @@
 		'amount': 'pod:Amount'
 	}
 
 	def __init__(self):
 		self._mosaic_id = UnresolvedMosaicId()
 		self._amount = Amount()
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def mosaic_id(self) -> UnresolvedMosaicId:
 		return self._mosaic_id
 
 	@property
 	def amount(self) -> Amount:
 		return self._amount
@@ -550,14 +556,17 @@
 		self._network = NetworkType.MAINNET
 		self._type_ = TransactionType.ACCOUNT_KEY_LINK
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -701,14 +710,17 @@
 		self._signer_public_key = PublicKey()
 		self._version = 0
 		self._network = NetworkType.MAINNET
 		self._type_ = TransactionType.ACCOUNT_KEY_LINK
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -795,15 +807,3577 @@
 		result += f'version: 0x{self._version:X}, '
 		result += f'network: {self._network.__str__()}, '
 		result += f'type_: {self._type_.__str__()}, '
 		result += ')'
 		return result
 
 
-class AccountKeyLinkTransaction:
+class ProofGamma(ByteArray):
+	SIZE = 32
+
+	def __init__(self, proof_gamma: StrBytes = bytes(32)):
+		super().__init__(self.SIZE, proof_gamma, ProofGamma)
+
+	@property
+	def size(self) -> int:
+		return 32
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> ProofGamma:
+		buffer = memoryview(payload)
+		return ProofGamma(ArrayHelpers.get_bytes(buffer, 32))
+
+	def serialize(self) -> bytes:
+		return self.bytes
+
+
+class ProofVerificationHash(ByteArray):
+	SIZE = 16
+
+	def __init__(self, proof_verification_hash: StrBytes = bytes(16)):
+		super().__init__(self.SIZE, proof_verification_hash, ProofVerificationHash)
+
+	@property
+	def size(self) -> int:
+		return 16
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> ProofVerificationHash:
+		buffer = memoryview(payload)
+		return ProofVerificationHash(ArrayHelpers.get_bytes(buffer, 16))
+
+	def serialize(self) -> bytes:
+		return self.bytes
+
+
+class ProofScalar(ByteArray):
+	SIZE = 32
+
+	def __init__(self, proof_scalar: StrBytes = bytes(32)):
+		super().__init__(self.SIZE, proof_scalar, ProofScalar)
+
+	@property
+	def size(self) -> int:
+		return 32
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> ProofScalar:
+		buffer = memoryview(payload)
+		return ProofScalar(ArrayHelpers.get_bytes(buffer, 32))
+
+	def serialize(self) -> bytes:
+		return self.bytes
+
+
+class BlockType(Enum):
+	NEMESIS = 32835
+	NORMAL = 33091
+	IMPORTANCE = 33347
+
+	@property
+	def size(self) -> int:
+		return 2
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> BlockType:
+		buffer = memoryview(payload)
+		return BlockType(int.from_bytes(buffer[:2], byteorder='little', signed=False))
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.value.to_bytes(2, byteorder='little', signed=False)
+		return buffer
+
+
+class VrfProof:
+	TYPE_HINTS = {
+		'gamma': 'pod:ProofGamma',
+		'verification_hash': 'pod:ProofVerificationHash',
+		'scalar': 'pod:ProofScalar'
+	}
+
+	def __init__(self):
+		self._gamma = ProofGamma()
+		self._verification_hash = ProofVerificationHash()
+		self._scalar = ProofScalar()
+
+	def sort(self) -> None:
+		pass
+
+	@property
+	def gamma(self) -> ProofGamma:
+		return self._gamma
+
+	@property
+	def verification_hash(self) -> ProofVerificationHash:
+		return self._verification_hash
+
+	@property
+	def scalar(self) -> ProofScalar:
+		return self._scalar
+
+	@gamma.setter
+	def gamma(self, value: ProofGamma):
+		self._gamma = value
+
+	@verification_hash.setter
+	def verification_hash(self, value: ProofVerificationHash):
+		self._verification_hash = value
+
+	@scalar.setter
+	def scalar(self, value: ProofScalar):
+		self._scalar = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += self.gamma.size
+		size += self.verification_hash.size
+		size += self.scalar.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> VrfProof:
+		buffer = memoryview(payload)
+		gamma = ProofGamma.deserialize(buffer)
+		buffer = buffer[gamma.size:]
+		verification_hash = ProofVerificationHash.deserialize(buffer)
+		buffer = buffer[verification_hash.size:]
+		scalar = ProofScalar.deserialize(buffer)
+		buffer = buffer[scalar.size:]
+
+		instance = VrfProof()
+		instance._gamma = gamma
+		instance._verification_hash = verification_hash
+		instance._scalar = scalar
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self._gamma.serialize()
+		buffer += self._verification_hash.serialize()
+		buffer += self._scalar.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'gamma: {self._gamma.__str__()}, '
+		result += f'verification_hash: {self._verification_hash.__str__()}, '
+		result += f'scalar: {self._scalar.__str__()}, '
+		result += ')'
+		return result
+
+
+class Block:
+	TYPE_HINTS = {
+		'signature': 'pod:Signature',
+		'signer_public_key': 'pod:PublicKey',
+		'network': 'enum:NetworkType',
+		'type_': 'enum:BlockType',
+		'height': 'pod:Height',
+		'timestamp': 'pod:Timestamp',
+		'difficulty': 'pod:Difficulty',
+		'generation_hash_proof': 'struct:VrfProof',
+		'previous_block_hash': 'pod:Hash256',
+		'transactions_hash': 'pod:Hash256',
+		'receipts_hash': 'pod:Hash256',
+		'state_hash': 'pod:Hash256',
+		'beneficiary_address': 'pod:Address',
+		'fee_multiplier': 'pod:BlockFeeMultiplier'
+	}
+
+	def __init__(self):
+		self._signature = Signature()
+		self._signer_public_key = PublicKey()
+		self._version = 0
+		self._network = NetworkType.MAINNET
+		self._type_ = BlockType.NEMESIS
+		self._height = Height()
+		self._timestamp = Timestamp()
+		self._difficulty = Difficulty()
+		self._generation_hash_proof = VrfProof()
+		self._previous_block_hash = Hash256()
+		self._transactions_hash = Hash256()
+		self._receipts_hash = Hash256()
+		self._state_hash = Hash256()
+		self._beneficiary_address = Address()
+		self._fee_multiplier = BlockFeeMultiplier()
+		self._verifiable_entity_header_reserved_1 = 0  # reserved field
+		self._entity_body_reserved_1 = 0  # reserved field
+
+	def sort(self) -> None:
+		self._generation_hash_proof.sort()
+
+	@property
+	def signature(self) -> Signature:
+		return self._signature
+
+	@property
+	def signer_public_key(self) -> PublicKey:
+		return self._signer_public_key
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def network(self) -> NetworkType:
+		return self._network
+
+	@property
+	def type_(self) -> BlockType:
+		return self._type_
+
+	@property
+	def height(self) -> Height:
+		return self._height
+
+	@property
+	def timestamp(self) -> Timestamp:
+		return self._timestamp
+
+	@property
+	def difficulty(self) -> Difficulty:
+		return self._difficulty
+
+	@property
+	def generation_hash_proof(self) -> VrfProof:
+		return self._generation_hash_proof
+
+	@property
+	def previous_block_hash(self) -> Hash256:
+		return self._previous_block_hash
+
+	@property
+	def transactions_hash(self) -> Hash256:
+		return self._transactions_hash
+
+	@property
+	def receipts_hash(self) -> Hash256:
+		return self._receipts_hash
+
+	@property
+	def state_hash(self) -> Hash256:
+		return self._state_hash
+
+	@property
+	def beneficiary_address(self) -> Address:
+		return self._beneficiary_address
+
+	@property
+	def fee_multiplier(self) -> BlockFeeMultiplier:
+		return self._fee_multiplier
+
+	@signature.setter
+	def signature(self, value: Signature):
+		self._signature = value
+
+	@signer_public_key.setter
+	def signer_public_key(self, value: PublicKey):
+		self._signer_public_key = value
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@network.setter
+	def network(self, value: NetworkType):
+		self._network = value
+
+	@type_.setter
+	def type_(self, value: BlockType):
+		self._type_ = value
+
+	@height.setter
+	def height(self, value: Height):
+		self._height = value
+
+	@timestamp.setter
+	def timestamp(self, value: Timestamp):
+		self._timestamp = value
+
+	@difficulty.setter
+	def difficulty(self, value: Difficulty):
+		self._difficulty = value
+
+	@generation_hash_proof.setter
+	def generation_hash_proof(self, value: VrfProof):
+		self._generation_hash_proof = value
+
+	@previous_block_hash.setter
+	def previous_block_hash(self, value: Hash256):
+		self._previous_block_hash = value
+
+	@transactions_hash.setter
+	def transactions_hash(self, value: Hash256):
+		self._transactions_hash = value
+
+	@receipts_hash.setter
+	def receipts_hash(self, value: Hash256):
+		self._receipts_hash = value
+
+	@state_hash.setter
+	def state_hash(self, value: Hash256):
+		self._state_hash = value
+
+	@beneficiary_address.setter
+	def beneficiary_address(self, value: Address):
+		self._beneficiary_address = value
+
+	@fee_multiplier.setter
+	def fee_multiplier(self, value: BlockFeeMultiplier):
+		self._fee_multiplier = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 4
+		size += self.signature.size
+		size += self.signer_public_key.size
+		size += 4
+		size += 1
+		size += self.network.size
+		size += self.type_.size
+		size += self.height.size
+		size += self.timestamp.size
+		size += self.difficulty.size
+		size += self.generation_hash_proof.size
+		size += self.previous_block_hash.size
+		size += self.transactions_hash.size
+		size += self.receipts_hash.size
+		size += self.state_hash.size
+		size += self.beneficiary_address.size
+		size += self.fee_multiplier.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> Block:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert verifiable_entity_header_reserved_1 == 0, f'Invalid value of reserved field ({verifiable_entity_header_reserved_1})'
+		signature = Signature.deserialize(buffer)
+		buffer = buffer[signature.size:]
+		signer_public_key = PublicKey.deserialize(buffer)
+		buffer = buffer[signer_public_key.size:]
+		entity_body_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert entity_body_reserved_1 == 0, f'Invalid value of reserved field ({entity_body_reserved_1})'
+		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
+		buffer = buffer[1:]
+		network = NetworkType.deserialize(buffer)
+		buffer = buffer[network.size:]
+		type_ = BlockType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		height = Height.deserialize(buffer)
+		buffer = buffer[height.size:]
+		timestamp = Timestamp.deserialize(buffer)
+		buffer = buffer[timestamp.size:]
+		difficulty = Difficulty.deserialize(buffer)
+		buffer = buffer[difficulty.size:]
+		generation_hash_proof = VrfProof.deserialize(buffer)
+		buffer = buffer[generation_hash_proof.size:]
+		previous_block_hash = Hash256.deserialize(buffer)
+		buffer = buffer[previous_block_hash.size:]
+		transactions_hash = Hash256.deserialize(buffer)
+		buffer = buffer[transactions_hash.size:]
+		receipts_hash = Hash256.deserialize(buffer)
+		buffer = buffer[receipts_hash.size:]
+		state_hash = Hash256.deserialize(buffer)
+		buffer = buffer[state_hash.size:]
+		beneficiary_address = Address.deserialize(buffer)
+		buffer = buffer[beneficiary_address.size:]
+		fee_multiplier = BlockFeeMultiplier.deserialize(buffer)
+		buffer = buffer[fee_multiplier.size:]
+
+		instance = Block()
+		instance._signature = signature
+		instance._signer_public_key = signer_public_key
+		instance._version = version
+		instance._network = network
+		instance._type_ = type_
+		instance._height = height
+		instance._timestamp = timestamp
+		instance._difficulty = difficulty
+		instance._generation_hash_proof = generation_hash_proof
+		instance._previous_block_hash = previous_block_hash
+		instance._transactions_hash = transactions_hash
+		instance._receipts_hash = receipts_hash
+		instance._state_hash = state_hash
+		instance._beneficiary_address = beneficiary_address
+		instance._fee_multiplier = fee_multiplier
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._verifiable_entity_header_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._signature.serialize()
+		buffer += self._signer_public_key.serialize()
+		buffer += self._entity_body_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(1, byteorder='little', signed=False)
+		buffer += self._network.serialize()
+		buffer += self._type_.serialize()
+		buffer += self._height.serialize()
+		buffer += self._timestamp.serialize()
+		buffer += self._difficulty.serialize()
+		buffer += self._generation_hash_proof.serialize()
+		buffer += self._previous_block_hash.serialize()
+		buffer += self._transactions_hash.serialize()
+		buffer += self._receipts_hash.serialize()
+		buffer += self._state_hash.serialize()
+		buffer += self._beneficiary_address.serialize()
+		buffer += self._fee_multiplier.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'signature: {self._signature.__str__()}, '
+		result += f'signer_public_key: {self._signer_public_key.__str__()}, '
+		result += f'version: 0x{self._version:X}, '
+		result += f'network: {self._network.__str__()}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'height: {self._height.__str__()}, '
+		result += f'timestamp: {self._timestamp.__str__()}, '
+		result += f'difficulty: {self._difficulty.__str__()}, '
+		result += f'generation_hash_proof: {self._generation_hash_proof.__str__()}, '
+		result += f'previous_block_hash: {self._previous_block_hash.__str__()}, '
+		result += f'transactions_hash: {self._transactions_hash.__str__()}, '
+		result += f'receipts_hash: {self._receipts_hash.__str__()}, '
+		result += f'state_hash: {self._state_hash.__str__()}, '
+		result += f'beneficiary_address: {self._beneficiary_address.__str__()}, '
+		result += f'fee_multiplier: {self._fee_multiplier.__str__()}, '
+		result += ')'
+		return result
+
+
+class NemesisBlockV1:
+	BLOCK_VERSION: int = 1
+	BLOCK_TYPE: BlockType = BlockType.NEMESIS
+	TYPE_HINTS = {
+		'signature': 'pod:Signature',
+		'signer_public_key': 'pod:PublicKey',
+		'network': 'enum:NetworkType',
+		'type_': 'enum:BlockType',
+		'height': 'pod:Height',
+		'timestamp': 'pod:Timestamp',
+		'difficulty': 'pod:Difficulty',
+		'generation_hash_proof': 'struct:VrfProof',
+		'previous_block_hash': 'pod:Hash256',
+		'transactions_hash': 'pod:Hash256',
+		'receipts_hash': 'pod:Hash256',
+		'state_hash': 'pod:Hash256',
+		'beneficiary_address': 'pod:Address',
+		'fee_multiplier': 'pod:BlockFeeMultiplier',
+		'total_voting_balance': 'pod:Amount',
+		'previous_importance_block_hash': 'pod:Hash256',
+		'transactions': 'array[Transaction]'
+	}
+
+	def __init__(self):
+		self._signature = Signature()
+		self._signer_public_key = PublicKey()
+		self._version = NemesisBlockV1.BLOCK_VERSION
+		self._network = NetworkType.MAINNET
+		self._type_ = NemesisBlockV1.BLOCK_TYPE
+		self._height = Height()
+		self._timestamp = Timestamp()
+		self._difficulty = Difficulty()
+		self._generation_hash_proof = VrfProof()
+		self._previous_block_hash = Hash256()
+		self._transactions_hash = Hash256()
+		self._receipts_hash = Hash256()
+		self._state_hash = Hash256()
+		self._beneficiary_address = Address()
+		self._fee_multiplier = BlockFeeMultiplier()
+		self._voting_eligible_accounts_count = 0
+		self._harvesting_eligible_accounts_count = 0
+		self._total_voting_balance = Amount()
+		self._previous_importance_block_hash = Hash256()
+		self._transactions = []
+		self._verifiable_entity_header_reserved_1 = 0  # reserved field
+		self._entity_body_reserved_1 = 0  # reserved field
+
+	def sort(self) -> None:
+		self._generation_hash_proof.sort()
+
+	@property
+	def signature(self) -> Signature:
+		return self._signature
+
+	@property
+	def signer_public_key(self) -> PublicKey:
+		return self._signer_public_key
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def network(self) -> NetworkType:
+		return self._network
+
+	@property
+	def type_(self) -> BlockType:
+		return self._type_
+
+	@property
+	def height(self) -> Height:
+		return self._height
+
+	@property
+	def timestamp(self) -> Timestamp:
+		return self._timestamp
+
+	@property
+	def difficulty(self) -> Difficulty:
+		return self._difficulty
+
+	@property
+	def generation_hash_proof(self) -> VrfProof:
+		return self._generation_hash_proof
+
+	@property
+	def previous_block_hash(self) -> Hash256:
+		return self._previous_block_hash
+
+	@property
+	def transactions_hash(self) -> Hash256:
+		return self._transactions_hash
+
+	@property
+	def receipts_hash(self) -> Hash256:
+		return self._receipts_hash
+
+	@property
+	def state_hash(self) -> Hash256:
+		return self._state_hash
+
+	@property
+	def beneficiary_address(self) -> Address:
+		return self._beneficiary_address
+
+	@property
+	def fee_multiplier(self) -> BlockFeeMultiplier:
+		return self._fee_multiplier
+
+	@property
+	def voting_eligible_accounts_count(self) -> int:
+		return self._voting_eligible_accounts_count
+
+	@property
+	def harvesting_eligible_accounts_count(self) -> int:
+		return self._harvesting_eligible_accounts_count
+
+	@property
+	def total_voting_balance(self) -> Amount:
+		return self._total_voting_balance
+
+	@property
+	def previous_importance_block_hash(self) -> Hash256:
+		return self._previous_importance_block_hash
+
+	@property
+	def transactions(self) -> List[Transaction]:
+		return self._transactions
+
+	@signature.setter
+	def signature(self, value: Signature):
+		self._signature = value
+
+	@signer_public_key.setter
+	def signer_public_key(self, value: PublicKey):
+		self._signer_public_key = value
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@network.setter
+	def network(self, value: NetworkType):
+		self._network = value
+
+	@type_.setter
+	def type_(self, value: BlockType):
+		self._type_ = value
+
+	@height.setter
+	def height(self, value: Height):
+		self._height = value
+
+	@timestamp.setter
+	def timestamp(self, value: Timestamp):
+		self._timestamp = value
+
+	@difficulty.setter
+	def difficulty(self, value: Difficulty):
+		self._difficulty = value
+
+	@generation_hash_proof.setter
+	def generation_hash_proof(self, value: VrfProof):
+		self._generation_hash_proof = value
+
+	@previous_block_hash.setter
+	def previous_block_hash(self, value: Hash256):
+		self._previous_block_hash = value
+
+	@transactions_hash.setter
+	def transactions_hash(self, value: Hash256):
+		self._transactions_hash = value
+
+	@receipts_hash.setter
+	def receipts_hash(self, value: Hash256):
+		self._receipts_hash = value
+
+	@state_hash.setter
+	def state_hash(self, value: Hash256):
+		self._state_hash = value
+
+	@beneficiary_address.setter
+	def beneficiary_address(self, value: Address):
+		self._beneficiary_address = value
+
+	@fee_multiplier.setter
+	def fee_multiplier(self, value: BlockFeeMultiplier):
+		self._fee_multiplier = value
+
+	@voting_eligible_accounts_count.setter
+	def voting_eligible_accounts_count(self, value: int):
+		self._voting_eligible_accounts_count = value
+
+	@harvesting_eligible_accounts_count.setter
+	def harvesting_eligible_accounts_count(self, value: int):
+		self._harvesting_eligible_accounts_count = value
+
+	@total_voting_balance.setter
+	def total_voting_balance(self, value: Amount):
+		self._total_voting_balance = value
+
+	@previous_importance_block_hash.setter
+	def previous_importance_block_hash(self, value: Hash256):
+		self._previous_importance_block_hash = value
+
+	@transactions.setter
+	def transactions(self, value: List[Transaction]):
+		self._transactions = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 4
+		size += self.signature.size
+		size += self.signer_public_key.size
+		size += 4
+		size += 1
+		size += self.network.size
+		size += self.type_.size
+		size += self.height.size
+		size += self.timestamp.size
+		size += self.difficulty.size
+		size += self.generation_hash_proof.size
+		size += self.previous_block_hash.size
+		size += self.transactions_hash.size
+		size += self.receipts_hash.size
+		size += self.state_hash.size
+		size += self.beneficiary_address.size
+		size += self.fee_multiplier.size
+		size += 4
+		size += 8
+		size += self.total_voting_balance.size
+		size += self.previous_importance_block_hash.size
+		size += ArrayHelpers.size(self.transactions, 8, skip_last_element_padding=True)
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> NemesisBlockV1:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert verifiable_entity_header_reserved_1 == 0, f'Invalid value of reserved field ({verifiable_entity_header_reserved_1})'
+		signature = Signature.deserialize(buffer)
+		buffer = buffer[signature.size:]
+		signer_public_key = PublicKey.deserialize(buffer)
+		buffer = buffer[signer_public_key.size:]
+		entity_body_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert entity_body_reserved_1 == 0, f'Invalid value of reserved field ({entity_body_reserved_1})'
+		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
+		buffer = buffer[1:]
+		network = NetworkType.deserialize(buffer)
+		buffer = buffer[network.size:]
+		type_ = BlockType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		height = Height.deserialize(buffer)
+		buffer = buffer[height.size:]
+		timestamp = Timestamp.deserialize(buffer)
+		buffer = buffer[timestamp.size:]
+		difficulty = Difficulty.deserialize(buffer)
+		buffer = buffer[difficulty.size:]
+		generation_hash_proof = VrfProof.deserialize(buffer)
+		buffer = buffer[generation_hash_proof.size:]
+		previous_block_hash = Hash256.deserialize(buffer)
+		buffer = buffer[previous_block_hash.size:]
+		transactions_hash = Hash256.deserialize(buffer)
+		buffer = buffer[transactions_hash.size:]
+		receipts_hash = Hash256.deserialize(buffer)
+		buffer = buffer[receipts_hash.size:]
+		state_hash = Hash256.deserialize(buffer)
+		buffer = buffer[state_hash.size:]
+		beneficiary_address = Address.deserialize(buffer)
+		buffer = buffer[beneficiary_address.size:]
+		fee_multiplier = BlockFeeMultiplier.deserialize(buffer)
+		buffer = buffer[fee_multiplier.size:]
+		voting_eligible_accounts_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		harvesting_eligible_accounts_count = int.from_bytes(buffer[:8], byteorder='little', signed=False)
+		buffer = buffer[8:]
+		total_voting_balance = Amount.deserialize(buffer)
+		buffer = buffer[total_voting_balance.size:]
+		previous_importance_block_hash = Hash256.deserialize(buffer)
+		buffer = buffer[previous_importance_block_hash.size:]
+		transactions = ArrayHelpers.read_variable_size_elements(buffer, TransactionFactory, 8, skip_last_element_padding=True)
+		buffer = buffer[ArrayHelpers.size(transactions, 8, skip_last_element_padding=True):]
+
+		instance = NemesisBlockV1()
+		instance._signature = signature
+		instance._signer_public_key = signer_public_key
+		instance._version = version
+		instance._network = network
+		instance._type_ = type_
+		instance._height = height
+		instance._timestamp = timestamp
+		instance._difficulty = difficulty
+		instance._generation_hash_proof = generation_hash_proof
+		instance._previous_block_hash = previous_block_hash
+		instance._transactions_hash = transactions_hash
+		instance._receipts_hash = receipts_hash
+		instance._state_hash = state_hash
+		instance._beneficiary_address = beneficiary_address
+		instance._fee_multiplier = fee_multiplier
+		instance._voting_eligible_accounts_count = voting_eligible_accounts_count
+		instance._harvesting_eligible_accounts_count = harvesting_eligible_accounts_count
+		instance._total_voting_balance = total_voting_balance
+		instance._previous_importance_block_hash = previous_importance_block_hash
+		instance._transactions = transactions
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._verifiable_entity_header_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._signature.serialize()
+		buffer += self._signer_public_key.serialize()
+		buffer += self._entity_body_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(1, byteorder='little', signed=False)
+		buffer += self._network.serialize()
+		buffer += self._type_.serialize()
+		buffer += self._height.serialize()
+		buffer += self._timestamp.serialize()
+		buffer += self._difficulty.serialize()
+		buffer += self._generation_hash_proof.serialize()
+		buffer += self._previous_block_hash.serialize()
+		buffer += self._transactions_hash.serialize()
+		buffer += self._receipts_hash.serialize()
+		buffer += self._state_hash.serialize()
+		buffer += self._beneficiary_address.serialize()
+		buffer += self._fee_multiplier.serialize()
+		buffer += self._voting_eligible_accounts_count.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._harvesting_eligible_accounts_count.to_bytes(8, byteorder='little', signed=False)
+		buffer += self._total_voting_balance.serialize()
+		buffer += self._previous_importance_block_hash.serialize()
+		buffer += ArrayHelpers.write_variable_size_elements(self._transactions, 8, skip_last_element_padding=True)
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'signature: {self._signature.__str__()}, '
+		result += f'signer_public_key: {self._signer_public_key.__str__()}, '
+		result += f'version: 0x{self._version:X}, '
+		result += f'network: {self._network.__str__()}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'height: {self._height.__str__()}, '
+		result += f'timestamp: {self._timestamp.__str__()}, '
+		result += f'difficulty: {self._difficulty.__str__()}, '
+		result += f'generation_hash_proof: {self._generation_hash_proof.__str__()}, '
+		result += f'previous_block_hash: {self._previous_block_hash.__str__()}, '
+		result += f'transactions_hash: {self._transactions_hash.__str__()}, '
+		result += f'receipts_hash: {self._receipts_hash.__str__()}, '
+		result += f'state_hash: {self._state_hash.__str__()}, '
+		result += f'beneficiary_address: {self._beneficiary_address.__str__()}, '
+		result += f'fee_multiplier: {self._fee_multiplier.__str__()}, '
+		result += f'voting_eligible_accounts_count: 0x{self._voting_eligible_accounts_count:X}, '
+		result += f'harvesting_eligible_accounts_count: 0x{self._harvesting_eligible_accounts_count:X}, '
+		result += f'total_voting_balance: {self._total_voting_balance.__str__()}, '
+		result += f'previous_importance_block_hash: {self._previous_importance_block_hash.__str__()}, '
+		result += f'transactions: {list(map(str, self._transactions))}, '
+		result += ')'
+		return result
+
+
+class NormalBlockV1:
+	BLOCK_VERSION: int = 1
+	BLOCK_TYPE: BlockType = BlockType.NORMAL
+	TYPE_HINTS = {
+		'signature': 'pod:Signature',
+		'signer_public_key': 'pod:PublicKey',
+		'network': 'enum:NetworkType',
+		'type_': 'enum:BlockType',
+		'height': 'pod:Height',
+		'timestamp': 'pod:Timestamp',
+		'difficulty': 'pod:Difficulty',
+		'generation_hash_proof': 'struct:VrfProof',
+		'previous_block_hash': 'pod:Hash256',
+		'transactions_hash': 'pod:Hash256',
+		'receipts_hash': 'pod:Hash256',
+		'state_hash': 'pod:Hash256',
+		'beneficiary_address': 'pod:Address',
+		'fee_multiplier': 'pod:BlockFeeMultiplier',
+		'transactions': 'array[Transaction]'
+	}
+
+	def __init__(self):
+		self._signature = Signature()
+		self._signer_public_key = PublicKey()
+		self._version = NormalBlockV1.BLOCK_VERSION
+		self._network = NetworkType.MAINNET
+		self._type_ = NormalBlockV1.BLOCK_TYPE
+		self._height = Height()
+		self._timestamp = Timestamp()
+		self._difficulty = Difficulty()
+		self._generation_hash_proof = VrfProof()
+		self._previous_block_hash = Hash256()
+		self._transactions_hash = Hash256()
+		self._receipts_hash = Hash256()
+		self._state_hash = Hash256()
+		self._beneficiary_address = Address()
+		self._fee_multiplier = BlockFeeMultiplier()
+		self._transactions = []
+		self._verifiable_entity_header_reserved_1 = 0  # reserved field
+		self._entity_body_reserved_1 = 0  # reserved field
+		self._block_header_reserved_1 = 0  # reserved field
+
+	def sort(self) -> None:
+		self._generation_hash_proof.sort()
+
+	@property
+	def signature(self) -> Signature:
+		return self._signature
+
+	@property
+	def signer_public_key(self) -> PublicKey:
+		return self._signer_public_key
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def network(self) -> NetworkType:
+		return self._network
+
+	@property
+	def type_(self) -> BlockType:
+		return self._type_
+
+	@property
+	def height(self) -> Height:
+		return self._height
+
+	@property
+	def timestamp(self) -> Timestamp:
+		return self._timestamp
+
+	@property
+	def difficulty(self) -> Difficulty:
+		return self._difficulty
+
+	@property
+	def generation_hash_proof(self) -> VrfProof:
+		return self._generation_hash_proof
+
+	@property
+	def previous_block_hash(self) -> Hash256:
+		return self._previous_block_hash
+
+	@property
+	def transactions_hash(self) -> Hash256:
+		return self._transactions_hash
+
+	@property
+	def receipts_hash(self) -> Hash256:
+		return self._receipts_hash
+
+	@property
+	def state_hash(self) -> Hash256:
+		return self._state_hash
+
+	@property
+	def beneficiary_address(self) -> Address:
+		return self._beneficiary_address
+
+	@property
+	def fee_multiplier(self) -> BlockFeeMultiplier:
+		return self._fee_multiplier
+
+	@property
+	def transactions(self) -> List[Transaction]:
+		return self._transactions
+
+	@signature.setter
+	def signature(self, value: Signature):
+		self._signature = value
+
+	@signer_public_key.setter
+	def signer_public_key(self, value: PublicKey):
+		self._signer_public_key = value
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@network.setter
+	def network(self, value: NetworkType):
+		self._network = value
+
+	@type_.setter
+	def type_(self, value: BlockType):
+		self._type_ = value
+
+	@height.setter
+	def height(self, value: Height):
+		self._height = value
+
+	@timestamp.setter
+	def timestamp(self, value: Timestamp):
+		self._timestamp = value
+
+	@difficulty.setter
+	def difficulty(self, value: Difficulty):
+		self._difficulty = value
+
+	@generation_hash_proof.setter
+	def generation_hash_proof(self, value: VrfProof):
+		self._generation_hash_proof = value
+
+	@previous_block_hash.setter
+	def previous_block_hash(self, value: Hash256):
+		self._previous_block_hash = value
+
+	@transactions_hash.setter
+	def transactions_hash(self, value: Hash256):
+		self._transactions_hash = value
+
+	@receipts_hash.setter
+	def receipts_hash(self, value: Hash256):
+		self._receipts_hash = value
+
+	@state_hash.setter
+	def state_hash(self, value: Hash256):
+		self._state_hash = value
+
+	@beneficiary_address.setter
+	def beneficiary_address(self, value: Address):
+		self._beneficiary_address = value
+
+	@fee_multiplier.setter
+	def fee_multiplier(self, value: BlockFeeMultiplier):
+		self._fee_multiplier = value
+
+	@transactions.setter
+	def transactions(self, value: List[Transaction]):
+		self._transactions = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 4
+		size += self.signature.size
+		size += self.signer_public_key.size
+		size += 4
+		size += 1
+		size += self.network.size
+		size += self.type_.size
+		size += self.height.size
+		size += self.timestamp.size
+		size += self.difficulty.size
+		size += self.generation_hash_proof.size
+		size += self.previous_block_hash.size
+		size += self.transactions_hash.size
+		size += self.receipts_hash.size
+		size += self.state_hash.size
+		size += self.beneficiary_address.size
+		size += self.fee_multiplier.size
+		size += 4
+		size += ArrayHelpers.size(self.transactions, 8, skip_last_element_padding=True)
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> NormalBlockV1:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert verifiable_entity_header_reserved_1 == 0, f'Invalid value of reserved field ({verifiable_entity_header_reserved_1})'
+		signature = Signature.deserialize(buffer)
+		buffer = buffer[signature.size:]
+		signer_public_key = PublicKey.deserialize(buffer)
+		buffer = buffer[signer_public_key.size:]
+		entity_body_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert entity_body_reserved_1 == 0, f'Invalid value of reserved field ({entity_body_reserved_1})'
+		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
+		buffer = buffer[1:]
+		network = NetworkType.deserialize(buffer)
+		buffer = buffer[network.size:]
+		type_ = BlockType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		height = Height.deserialize(buffer)
+		buffer = buffer[height.size:]
+		timestamp = Timestamp.deserialize(buffer)
+		buffer = buffer[timestamp.size:]
+		difficulty = Difficulty.deserialize(buffer)
+		buffer = buffer[difficulty.size:]
+		generation_hash_proof = VrfProof.deserialize(buffer)
+		buffer = buffer[generation_hash_proof.size:]
+		previous_block_hash = Hash256.deserialize(buffer)
+		buffer = buffer[previous_block_hash.size:]
+		transactions_hash = Hash256.deserialize(buffer)
+		buffer = buffer[transactions_hash.size:]
+		receipts_hash = Hash256.deserialize(buffer)
+		buffer = buffer[receipts_hash.size:]
+		state_hash = Hash256.deserialize(buffer)
+		buffer = buffer[state_hash.size:]
+		beneficiary_address = Address.deserialize(buffer)
+		buffer = buffer[beneficiary_address.size:]
+		fee_multiplier = BlockFeeMultiplier.deserialize(buffer)
+		buffer = buffer[fee_multiplier.size:]
+		block_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert block_header_reserved_1 == 0, f'Invalid value of reserved field ({block_header_reserved_1})'
+		transactions = ArrayHelpers.read_variable_size_elements(buffer, TransactionFactory, 8, skip_last_element_padding=True)
+		buffer = buffer[ArrayHelpers.size(transactions, 8, skip_last_element_padding=True):]
+
+		instance = NormalBlockV1()
+		instance._signature = signature
+		instance._signer_public_key = signer_public_key
+		instance._version = version
+		instance._network = network
+		instance._type_ = type_
+		instance._height = height
+		instance._timestamp = timestamp
+		instance._difficulty = difficulty
+		instance._generation_hash_proof = generation_hash_proof
+		instance._previous_block_hash = previous_block_hash
+		instance._transactions_hash = transactions_hash
+		instance._receipts_hash = receipts_hash
+		instance._state_hash = state_hash
+		instance._beneficiary_address = beneficiary_address
+		instance._fee_multiplier = fee_multiplier
+		instance._transactions = transactions
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._verifiable_entity_header_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._signature.serialize()
+		buffer += self._signer_public_key.serialize()
+		buffer += self._entity_body_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(1, byteorder='little', signed=False)
+		buffer += self._network.serialize()
+		buffer += self._type_.serialize()
+		buffer += self._height.serialize()
+		buffer += self._timestamp.serialize()
+		buffer += self._difficulty.serialize()
+		buffer += self._generation_hash_proof.serialize()
+		buffer += self._previous_block_hash.serialize()
+		buffer += self._transactions_hash.serialize()
+		buffer += self._receipts_hash.serialize()
+		buffer += self._state_hash.serialize()
+		buffer += self._beneficiary_address.serialize()
+		buffer += self._fee_multiplier.serialize()
+		buffer += self._block_header_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += ArrayHelpers.write_variable_size_elements(self._transactions, 8, skip_last_element_padding=True)
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'signature: {self._signature.__str__()}, '
+		result += f'signer_public_key: {self._signer_public_key.__str__()}, '
+		result += f'version: 0x{self._version:X}, '
+		result += f'network: {self._network.__str__()}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'height: {self._height.__str__()}, '
+		result += f'timestamp: {self._timestamp.__str__()}, '
+		result += f'difficulty: {self._difficulty.__str__()}, '
+		result += f'generation_hash_proof: {self._generation_hash_proof.__str__()}, '
+		result += f'previous_block_hash: {self._previous_block_hash.__str__()}, '
+		result += f'transactions_hash: {self._transactions_hash.__str__()}, '
+		result += f'receipts_hash: {self._receipts_hash.__str__()}, '
+		result += f'state_hash: {self._state_hash.__str__()}, '
+		result += f'beneficiary_address: {self._beneficiary_address.__str__()}, '
+		result += f'fee_multiplier: {self._fee_multiplier.__str__()}, '
+		result += f'transactions: {list(map(str, self._transactions))}, '
+		result += ')'
+		return result
+
+
+class ImportanceBlockV1:
+	BLOCK_VERSION: int = 1
+	BLOCK_TYPE: BlockType = BlockType.IMPORTANCE
+	TYPE_HINTS = {
+		'signature': 'pod:Signature',
+		'signer_public_key': 'pod:PublicKey',
+		'network': 'enum:NetworkType',
+		'type_': 'enum:BlockType',
+		'height': 'pod:Height',
+		'timestamp': 'pod:Timestamp',
+		'difficulty': 'pod:Difficulty',
+		'generation_hash_proof': 'struct:VrfProof',
+		'previous_block_hash': 'pod:Hash256',
+		'transactions_hash': 'pod:Hash256',
+		'receipts_hash': 'pod:Hash256',
+		'state_hash': 'pod:Hash256',
+		'beneficiary_address': 'pod:Address',
+		'fee_multiplier': 'pod:BlockFeeMultiplier',
+		'total_voting_balance': 'pod:Amount',
+		'previous_importance_block_hash': 'pod:Hash256',
+		'transactions': 'array[Transaction]'
+	}
+
+	def __init__(self):
+		self._signature = Signature()
+		self._signer_public_key = PublicKey()
+		self._version = ImportanceBlockV1.BLOCK_VERSION
+		self._network = NetworkType.MAINNET
+		self._type_ = ImportanceBlockV1.BLOCK_TYPE
+		self._height = Height()
+		self._timestamp = Timestamp()
+		self._difficulty = Difficulty()
+		self._generation_hash_proof = VrfProof()
+		self._previous_block_hash = Hash256()
+		self._transactions_hash = Hash256()
+		self._receipts_hash = Hash256()
+		self._state_hash = Hash256()
+		self._beneficiary_address = Address()
+		self._fee_multiplier = BlockFeeMultiplier()
+		self._voting_eligible_accounts_count = 0
+		self._harvesting_eligible_accounts_count = 0
+		self._total_voting_balance = Amount()
+		self._previous_importance_block_hash = Hash256()
+		self._transactions = []
+		self._verifiable_entity_header_reserved_1 = 0  # reserved field
+		self._entity_body_reserved_1 = 0  # reserved field
+
+	def sort(self) -> None:
+		self._generation_hash_proof.sort()
+
+	@property
+	def signature(self) -> Signature:
+		return self._signature
+
+	@property
+	def signer_public_key(self) -> PublicKey:
+		return self._signer_public_key
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def network(self) -> NetworkType:
+		return self._network
+
+	@property
+	def type_(self) -> BlockType:
+		return self._type_
+
+	@property
+	def height(self) -> Height:
+		return self._height
+
+	@property
+	def timestamp(self) -> Timestamp:
+		return self._timestamp
+
+	@property
+	def difficulty(self) -> Difficulty:
+		return self._difficulty
+
+	@property
+	def generation_hash_proof(self) -> VrfProof:
+		return self._generation_hash_proof
+
+	@property
+	def previous_block_hash(self) -> Hash256:
+		return self._previous_block_hash
+
+	@property
+	def transactions_hash(self) -> Hash256:
+		return self._transactions_hash
+
+	@property
+	def receipts_hash(self) -> Hash256:
+		return self._receipts_hash
+
+	@property
+	def state_hash(self) -> Hash256:
+		return self._state_hash
+
+	@property
+	def beneficiary_address(self) -> Address:
+		return self._beneficiary_address
+
+	@property
+	def fee_multiplier(self) -> BlockFeeMultiplier:
+		return self._fee_multiplier
+
+	@property
+	def voting_eligible_accounts_count(self) -> int:
+		return self._voting_eligible_accounts_count
+
+	@property
+	def harvesting_eligible_accounts_count(self) -> int:
+		return self._harvesting_eligible_accounts_count
+
+	@property
+	def total_voting_balance(self) -> Amount:
+		return self._total_voting_balance
+
+	@property
+	def previous_importance_block_hash(self) -> Hash256:
+		return self._previous_importance_block_hash
+
+	@property
+	def transactions(self) -> List[Transaction]:
+		return self._transactions
+
+	@signature.setter
+	def signature(self, value: Signature):
+		self._signature = value
+
+	@signer_public_key.setter
+	def signer_public_key(self, value: PublicKey):
+		self._signer_public_key = value
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@network.setter
+	def network(self, value: NetworkType):
+		self._network = value
+
+	@type_.setter
+	def type_(self, value: BlockType):
+		self._type_ = value
+
+	@height.setter
+	def height(self, value: Height):
+		self._height = value
+
+	@timestamp.setter
+	def timestamp(self, value: Timestamp):
+		self._timestamp = value
+
+	@difficulty.setter
+	def difficulty(self, value: Difficulty):
+		self._difficulty = value
+
+	@generation_hash_proof.setter
+	def generation_hash_proof(self, value: VrfProof):
+		self._generation_hash_proof = value
+
+	@previous_block_hash.setter
+	def previous_block_hash(self, value: Hash256):
+		self._previous_block_hash = value
+
+	@transactions_hash.setter
+	def transactions_hash(self, value: Hash256):
+		self._transactions_hash = value
+
+	@receipts_hash.setter
+	def receipts_hash(self, value: Hash256):
+		self._receipts_hash = value
+
+	@state_hash.setter
+	def state_hash(self, value: Hash256):
+		self._state_hash = value
+
+	@beneficiary_address.setter
+	def beneficiary_address(self, value: Address):
+		self._beneficiary_address = value
+
+	@fee_multiplier.setter
+	def fee_multiplier(self, value: BlockFeeMultiplier):
+		self._fee_multiplier = value
+
+	@voting_eligible_accounts_count.setter
+	def voting_eligible_accounts_count(self, value: int):
+		self._voting_eligible_accounts_count = value
+
+	@harvesting_eligible_accounts_count.setter
+	def harvesting_eligible_accounts_count(self, value: int):
+		self._harvesting_eligible_accounts_count = value
+
+	@total_voting_balance.setter
+	def total_voting_balance(self, value: Amount):
+		self._total_voting_balance = value
+
+	@previous_importance_block_hash.setter
+	def previous_importance_block_hash(self, value: Hash256):
+		self._previous_importance_block_hash = value
+
+	@transactions.setter
+	def transactions(self, value: List[Transaction]):
+		self._transactions = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 4
+		size += self.signature.size
+		size += self.signer_public_key.size
+		size += 4
+		size += 1
+		size += self.network.size
+		size += self.type_.size
+		size += self.height.size
+		size += self.timestamp.size
+		size += self.difficulty.size
+		size += self.generation_hash_proof.size
+		size += self.previous_block_hash.size
+		size += self.transactions_hash.size
+		size += self.receipts_hash.size
+		size += self.state_hash.size
+		size += self.beneficiary_address.size
+		size += self.fee_multiplier.size
+		size += 4
+		size += 8
+		size += self.total_voting_balance.size
+		size += self.previous_importance_block_hash.size
+		size += ArrayHelpers.size(self.transactions, 8, skip_last_element_padding=True)
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> ImportanceBlockV1:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert verifiable_entity_header_reserved_1 == 0, f'Invalid value of reserved field ({verifiable_entity_header_reserved_1})'
+		signature = Signature.deserialize(buffer)
+		buffer = buffer[signature.size:]
+		signer_public_key = PublicKey.deserialize(buffer)
+		buffer = buffer[signer_public_key.size:]
+		entity_body_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert entity_body_reserved_1 == 0, f'Invalid value of reserved field ({entity_body_reserved_1})'
+		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
+		buffer = buffer[1:]
+		network = NetworkType.deserialize(buffer)
+		buffer = buffer[network.size:]
+		type_ = BlockType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		height = Height.deserialize(buffer)
+		buffer = buffer[height.size:]
+		timestamp = Timestamp.deserialize(buffer)
+		buffer = buffer[timestamp.size:]
+		difficulty = Difficulty.deserialize(buffer)
+		buffer = buffer[difficulty.size:]
+		generation_hash_proof = VrfProof.deserialize(buffer)
+		buffer = buffer[generation_hash_proof.size:]
+		previous_block_hash = Hash256.deserialize(buffer)
+		buffer = buffer[previous_block_hash.size:]
+		transactions_hash = Hash256.deserialize(buffer)
+		buffer = buffer[transactions_hash.size:]
+		receipts_hash = Hash256.deserialize(buffer)
+		buffer = buffer[receipts_hash.size:]
+		state_hash = Hash256.deserialize(buffer)
+		buffer = buffer[state_hash.size:]
+		beneficiary_address = Address.deserialize(buffer)
+		buffer = buffer[beneficiary_address.size:]
+		fee_multiplier = BlockFeeMultiplier.deserialize(buffer)
+		buffer = buffer[fee_multiplier.size:]
+		voting_eligible_accounts_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		harvesting_eligible_accounts_count = int.from_bytes(buffer[:8], byteorder='little', signed=False)
+		buffer = buffer[8:]
+		total_voting_balance = Amount.deserialize(buffer)
+		buffer = buffer[total_voting_balance.size:]
+		previous_importance_block_hash = Hash256.deserialize(buffer)
+		buffer = buffer[previous_importance_block_hash.size:]
+		transactions = ArrayHelpers.read_variable_size_elements(buffer, TransactionFactory, 8, skip_last_element_padding=True)
+		buffer = buffer[ArrayHelpers.size(transactions, 8, skip_last_element_padding=True):]
+
+		instance = ImportanceBlockV1()
+		instance._signature = signature
+		instance._signer_public_key = signer_public_key
+		instance._version = version
+		instance._network = network
+		instance._type_ = type_
+		instance._height = height
+		instance._timestamp = timestamp
+		instance._difficulty = difficulty
+		instance._generation_hash_proof = generation_hash_proof
+		instance._previous_block_hash = previous_block_hash
+		instance._transactions_hash = transactions_hash
+		instance._receipts_hash = receipts_hash
+		instance._state_hash = state_hash
+		instance._beneficiary_address = beneficiary_address
+		instance._fee_multiplier = fee_multiplier
+		instance._voting_eligible_accounts_count = voting_eligible_accounts_count
+		instance._harvesting_eligible_accounts_count = harvesting_eligible_accounts_count
+		instance._total_voting_balance = total_voting_balance
+		instance._previous_importance_block_hash = previous_importance_block_hash
+		instance._transactions = transactions
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._verifiable_entity_header_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._signature.serialize()
+		buffer += self._signer_public_key.serialize()
+		buffer += self._entity_body_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(1, byteorder='little', signed=False)
+		buffer += self._network.serialize()
+		buffer += self._type_.serialize()
+		buffer += self._height.serialize()
+		buffer += self._timestamp.serialize()
+		buffer += self._difficulty.serialize()
+		buffer += self._generation_hash_proof.serialize()
+		buffer += self._previous_block_hash.serialize()
+		buffer += self._transactions_hash.serialize()
+		buffer += self._receipts_hash.serialize()
+		buffer += self._state_hash.serialize()
+		buffer += self._beneficiary_address.serialize()
+		buffer += self._fee_multiplier.serialize()
+		buffer += self._voting_eligible_accounts_count.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._harvesting_eligible_accounts_count.to_bytes(8, byteorder='little', signed=False)
+		buffer += self._total_voting_balance.serialize()
+		buffer += self._previous_importance_block_hash.serialize()
+		buffer += ArrayHelpers.write_variable_size_elements(self._transactions, 8, skip_last_element_padding=True)
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'signature: {self._signature.__str__()}, '
+		result += f'signer_public_key: {self._signer_public_key.__str__()}, '
+		result += f'version: 0x{self._version:X}, '
+		result += f'network: {self._network.__str__()}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'height: {self._height.__str__()}, '
+		result += f'timestamp: {self._timestamp.__str__()}, '
+		result += f'difficulty: {self._difficulty.__str__()}, '
+		result += f'generation_hash_proof: {self._generation_hash_proof.__str__()}, '
+		result += f'previous_block_hash: {self._previous_block_hash.__str__()}, '
+		result += f'transactions_hash: {self._transactions_hash.__str__()}, '
+		result += f'receipts_hash: {self._receipts_hash.__str__()}, '
+		result += f'state_hash: {self._state_hash.__str__()}, '
+		result += f'beneficiary_address: {self._beneficiary_address.__str__()}, '
+		result += f'fee_multiplier: {self._fee_multiplier.__str__()}, '
+		result += f'voting_eligible_accounts_count: 0x{self._voting_eligible_accounts_count:X}, '
+		result += f'harvesting_eligible_accounts_count: 0x{self._harvesting_eligible_accounts_count:X}, '
+		result += f'total_voting_balance: {self._total_voting_balance.__str__()}, '
+		result += f'previous_importance_block_hash: {self._previous_importance_block_hash.__str__()}, '
+		result += f'transactions: {list(map(str, self._transactions))}, '
+		result += ')'
+		return result
+
+
+class FinalizationRound:
+	TYPE_HINTS = {
+		'epoch': 'pod:FinalizationEpoch',
+		'point': 'pod:FinalizationPoint'
+	}
+
+	def __init__(self):
+		self._epoch = FinalizationEpoch()
+		self._point = FinalizationPoint()
+
+	def sort(self) -> None:
+		pass
+
+	@property
+	def epoch(self) -> FinalizationEpoch:
+		return self._epoch
+
+	@property
+	def point(self) -> FinalizationPoint:
+		return self._point
+
+	@epoch.setter
+	def epoch(self, value: FinalizationEpoch):
+		self._epoch = value
+
+	@point.setter
+	def point(self, value: FinalizationPoint):
+		self._point = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += self.epoch.size
+		size += self.point.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> FinalizationRound:
+		buffer = memoryview(payload)
+		epoch = FinalizationEpoch.deserialize(buffer)
+		buffer = buffer[epoch.size:]
+		point = FinalizationPoint.deserialize(buffer)
+		buffer = buffer[point.size:]
+
+		instance = FinalizationRound()
+		instance._epoch = epoch
+		instance._point = point
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self._epoch.serialize()
+		buffer += self._point.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'epoch: {self._epoch.__str__()}, '
+		result += f'point: {self._point.__str__()}, '
+		result += ')'
+		return result
+
+
+class FinalizedBlockHeader:
+	TYPE_HINTS = {
+		'round': 'struct:FinalizationRound',
+		'height': 'pod:Height',
+		'hash': 'pod:Hash256'
+	}
+
+	def __init__(self):
+		self._round = FinalizationRound()
+		self._height = Height()
+		self._hash = Hash256()
+
+	def sort(self) -> None:
+		self._round.sort()
+
+	@property
+	def round(self) -> FinalizationRound:
+		return self._round
+
+	@property
+	def height(self) -> Height:
+		return self._height
+
+	@property
+	def hash(self) -> Hash256:
+		return self._hash
+
+	@round.setter
+	def round(self, value: FinalizationRound):
+		self._round = value
+
+	@height.setter
+	def height(self, value: Height):
+		self._height = value
+
+	@hash.setter
+	def hash(self, value: Hash256):
+		self._hash = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += self.round.size
+		size += self.height.size
+		size += self.hash.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> FinalizedBlockHeader:
+		buffer = memoryview(payload)
+		round = FinalizationRound.deserialize(buffer)
+		buffer = buffer[round.size:]
+		height = Height.deserialize(buffer)
+		buffer = buffer[height.size:]
+		hash = Hash256.deserialize(buffer)
+		buffer = buffer[hash.size:]
+
+		instance = FinalizedBlockHeader()
+		instance._round = round
+		instance._height = height
+		instance._hash = hash
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self._round.serialize()
+		buffer += self._height.serialize()
+		buffer += self._hash.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'round: {self._round.__str__()}, '
+		result += f'height: {self._height.__str__()}, '
+		result += f'hash: {self._hash.__str__()}, '
+		result += ')'
+		return result
+
+
+class ReceiptType(Enum):
+	MOSAIC_RENTAL_FEE = 4685
+	NAMESPACE_RENTAL_FEE = 4942
+	HARVEST_FEE = 8515
+	LOCK_HASH_COMPLETED = 8776
+	LOCK_HASH_EXPIRED = 9032
+	LOCK_SECRET_COMPLETED = 8786
+	LOCK_SECRET_EXPIRED = 9042
+	LOCK_HASH_CREATED = 12616
+	LOCK_SECRET_CREATED = 12626
+	MOSAIC_EXPIRED = 16717
+	NAMESPACE_EXPIRED = 16718
+	NAMESPACE_DELETED = 16974
+	INFLATION = 20803
+	TRANSACTION_GROUP = 57667
+	ADDRESS_ALIAS_RESOLUTION = 61763
+	MOSAIC_ALIAS_RESOLUTION = 62019
+
+	@property
+	def size(self) -> int:
+		return 2
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> ReceiptType:
+		buffer = memoryview(payload)
+		return ReceiptType(int.from_bytes(buffer[:2], byteorder='little', signed=False))
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.value.to_bytes(2, byteorder='little', signed=False)
+		return buffer
+
+
+class Receipt:
+	TYPE_HINTS = {
+		'type_': 'enum:ReceiptType'
+	}
+
+	def __init__(self):
+		self._version = 0
+		self._type_ = ReceiptType.MOSAIC_RENTAL_FEE
+
+	def sort(self) -> None:
+		pass
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def type_(self) -> ReceiptType:
+		return self._type_
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@type_.setter
+	def type_(self, value: ReceiptType):
+		self._type_ = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 2
+		size += self.type_.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> Receipt:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		version = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		type_ = ReceiptType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+
+		instance = Receipt()
+		instance._version = version
+		instance._type_ = type_
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._type_.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'version: 0x{self._version:X}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += ')'
+		return result
+
+
+class HarvestFeeReceipt:
+	RECEIPT_TYPE: ReceiptType = ReceiptType.HARVEST_FEE
+	TYPE_HINTS = {
+		'type_': 'enum:ReceiptType',
+		'mosaic': 'struct:Mosaic',
+		'target_address': 'pod:Address'
+	}
+
+	def __init__(self):
+		self._version = 0
+		self._type_ = HarvestFeeReceipt.RECEIPT_TYPE
+		self._mosaic = Mosaic()
+		self._target_address = Address()
+
+	def sort(self) -> None:
+		self._mosaic.sort()
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def type_(self) -> ReceiptType:
+		return self._type_
+
+	@property
+	def mosaic(self) -> Mosaic:
+		return self._mosaic
+
+	@property
+	def target_address(self) -> Address:
+		return self._target_address
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@type_.setter
+	def type_(self, value: ReceiptType):
+		self._type_ = value
+
+	@mosaic.setter
+	def mosaic(self, value: Mosaic):
+		self._mosaic = value
+
+	@target_address.setter
+	def target_address(self, value: Address):
+		self._target_address = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 2
+		size += self.type_.size
+		size += self.mosaic.size
+		size += self.target_address.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> HarvestFeeReceipt:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		version = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		type_ = ReceiptType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		mosaic = Mosaic.deserialize(buffer)
+		buffer = buffer[mosaic.size:]
+		target_address = Address.deserialize(buffer)
+		buffer = buffer[target_address.size:]
+
+		instance = HarvestFeeReceipt()
+		instance._version = version
+		instance._type_ = type_
+		instance._mosaic = mosaic
+		instance._target_address = target_address
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._type_.serialize()
+		buffer += self._mosaic.serialize()
+		buffer += self._target_address.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'version: 0x{self._version:X}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'mosaic: {self._mosaic.__str__()}, '
+		result += f'target_address: {self._target_address.__str__()}, '
+		result += ')'
+		return result
+
+
+class InflationReceipt:
+	RECEIPT_TYPE: ReceiptType = ReceiptType.INFLATION
+	TYPE_HINTS = {
+		'type_': 'enum:ReceiptType',
+		'mosaic': 'struct:Mosaic'
+	}
+
+	def __init__(self):
+		self._version = 0
+		self._type_ = InflationReceipt.RECEIPT_TYPE
+		self._mosaic = Mosaic()
+
+	def sort(self) -> None:
+		self._mosaic.sort()
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def type_(self) -> ReceiptType:
+		return self._type_
+
+	@property
+	def mosaic(self) -> Mosaic:
+		return self._mosaic
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@type_.setter
+	def type_(self, value: ReceiptType):
+		self._type_ = value
+
+	@mosaic.setter
+	def mosaic(self, value: Mosaic):
+		self._mosaic = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 2
+		size += self.type_.size
+		size += self.mosaic.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> InflationReceipt:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		version = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		type_ = ReceiptType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		mosaic = Mosaic.deserialize(buffer)
+		buffer = buffer[mosaic.size:]
+
+		instance = InflationReceipt()
+		instance._version = version
+		instance._type_ = type_
+		instance._mosaic = mosaic
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._type_.serialize()
+		buffer += self._mosaic.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'version: 0x{self._version:X}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'mosaic: {self._mosaic.__str__()}, '
+		result += ')'
+		return result
+
+
+class LockHashCreatedFeeReceipt:
+	RECEIPT_TYPE: ReceiptType = ReceiptType.LOCK_HASH_CREATED
+	TYPE_HINTS = {
+		'type_': 'enum:ReceiptType',
+		'mosaic': 'struct:Mosaic',
+		'target_address': 'pod:Address'
+	}
+
+	def __init__(self):
+		self._version = 0
+		self._type_ = LockHashCreatedFeeReceipt.RECEIPT_TYPE
+		self._mosaic = Mosaic()
+		self._target_address = Address()
+
+	def sort(self) -> None:
+		self._mosaic.sort()
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def type_(self) -> ReceiptType:
+		return self._type_
+
+	@property
+	def mosaic(self) -> Mosaic:
+		return self._mosaic
+
+	@property
+	def target_address(self) -> Address:
+		return self._target_address
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@type_.setter
+	def type_(self, value: ReceiptType):
+		self._type_ = value
+
+	@mosaic.setter
+	def mosaic(self, value: Mosaic):
+		self._mosaic = value
+
+	@target_address.setter
+	def target_address(self, value: Address):
+		self._target_address = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 2
+		size += self.type_.size
+		size += self.mosaic.size
+		size += self.target_address.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> LockHashCreatedFeeReceipt:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		version = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		type_ = ReceiptType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		mosaic = Mosaic.deserialize(buffer)
+		buffer = buffer[mosaic.size:]
+		target_address = Address.deserialize(buffer)
+		buffer = buffer[target_address.size:]
+
+		instance = LockHashCreatedFeeReceipt()
+		instance._version = version
+		instance._type_ = type_
+		instance._mosaic = mosaic
+		instance._target_address = target_address
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._type_.serialize()
+		buffer += self._mosaic.serialize()
+		buffer += self._target_address.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'version: 0x{self._version:X}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'mosaic: {self._mosaic.__str__()}, '
+		result += f'target_address: {self._target_address.__str__()}, '
+		result += ')'
+		return result
+
+
+class LockHashCompletedFeeReceipt:
+	RECEIPT_TYPE: ReceiptType = ReceiptType.LOCK_HASH_COMPLETED
+	TYPE_HINTS = {
+		'type_': 'enum:ReceiptType',
+		'mosaic': 'struct:Mosaic',
+		'target_address': 'pod:Address'
+	}
+
+	def __init__(self):
+		self._version = 0
+		self._type_ = LockHashCompletedFeeReceipt.RECEIPT_TYPE
+		self._mosaic = Mosaic()
+		self._target_address = Address()
+
+	def sort(self) -> None:
+		self._mosaic.sort()
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def type_(self) -> ReceiptType:
+		return self._type_
+
+	@property
+	def mosaic(self) -> Mosaic:
+		return self._mosaic
+
+	@property
+	def target_address(self) -> Address:
+		return self._target_address
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@type_.setter
+	def type_(self, value: ReceiptType):
+		self._type_ = value
+
+	@mosaic.setter
+	def mosaic(self, value: Mosaic):
+		self._mosaic = value
+
+	@target_address.setter
+	def target_address(self, value: Address):
+		self._target_address = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 2
+		size += self.type_.size
+		size += self.mosaic.size
+		size += self.target_address.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> LockHashCompletedFeeReceipt:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		version = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		type_ = ReceiptType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		mosaic = Mosaic.deserialize(buffer)
+		buffer = buffer[mosaic.size:]
+		target_address = Address.deserialize(buffer)
+		buffer = buffer[target_address.size:]
+
+		instance = LockHashCompletedFeeReceipt()
+		instance._version = version
+		instance._type_ = type_
+		instance._mosaic = mosaic
+		instance._target_address = target_address
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._type_.serialize()
+		buffer += self._mosaic.serialize()
+		buffer += self._target_address.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'version: 0x{self._version:X}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'mosaic: {self._mosaic.__str__()}, '
+		result += f'target_address: {self._target_address.__str__()}, '
+		result += ')'
+		return result
+
+
+class LockHashExpiredFeeReceipt:
+	RECEIPT_TYPE: ReceiptType = ReceiptType.LOCK_HASH_EXPIRED
+	TYPE_HINTS = {
+		'type_': 'enum:ReceiptType',
+		'mosaic': 'struct:Mosaic',
+		'target_address': 'pod:Address'
+	}
+
+	def __init__(self):
+		self._version = 0
+		self._type_ = LockHashExpiredFeeReceipt.RECEIPT_TYPE
+		self._mosaic = Mosaic()
+		self._target_address = Address()
+
+	def sort(self) -> None:
+		self._mosaic.sort()
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def type_(self) -> ReceiptType:
+		return self._type_
+
+	@property
+	def mosaic(self) -> Mosaic:
+		return self._mosaic
+
+	@property
+	def target_address(self) -> Address:
+		return self._target_address
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@type_.setter
+	def type_(self, value: ReceiptType):
+		self._type_ = value
+
+	@mosaic.setter
+	def mosaic(self, value: Mosaic):
+		self._mosaic = value
+
+	@target_address.setter
+	def target_address(self, value: Address):
+		self._target_address = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 2
+		size += self.type_.size
+		size += self.mosaic.size
+		size += self.target_address.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> LockHashExpiredFeeReceipt:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		version = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		type_ = ReceiptType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		mosaic = Mosaic.deserialize(buffer)
+		buffer = buffer[mosaic.size:]
+		target_address = Address.deserialize(buffer)
+		buffer = buffer[target_address.size:]
+
+		instance = LockHashExpiredFeeReceipt()
+		instance._version = version
+		instance._type_ = type_
+		instance._mosaic = mosaic
+		instance._target_address = target_address
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._type_.serialize()
+		buffer += self._mosaic.serialize()
+		buffer += self._target_address.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'version: 0x{self._version:X}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'mosaic: {self._mosaic.__str__()}, '
+		result += f'target_address: {self._target_address.__str__()}, '
+		result += ')'
+		return result
+
+
+class LockSecretCreatedFeeReceipt:
+	RECEIPT_TYPE: ReceiptType = ReceiptType.LOCK_SECRET_CREATED
+	TYPE_HINTS = {
+		'type_': 'enum:ReceiptType',
+		'mosaic': 'struct:Mosaic',
+		'target_address': 'pod:Address'
+	}
+
+	def __init__(self):
+		self._version = 0
+		self._type_ = LockSecretCreatedFeeReceipt.RECEIPT_TYPE
+		self._mosaic = Mosaic()
+		self._target_address = Address()
+
+	def sort(self) -> None:
+		self._mosaic.sort()
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def type_(self) -> ReceiptType:
+		return self._type_
+
+	@property
+	def mosaic(self) -> Mosaic:
+		return self._mosaic
+
+	@property
+	def target_address(self) -> Address:
+		return self._target_address
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@type_.setter
+	def type_(self, value: ReceiptType):
+		self._type_ = value
+
+	@mosaic.setter
+	def mosaic(self, value: Mosaic):
+		self._mosaic = value
+
+	@target_address.setter
+	def target_address(self, value: Address):
+		self._target_address = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 2
+		size += self.type_.size
+		size += self.mosaic.size
+		size += self.target_address.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> LockSecretCreatedFeeReceipt:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		version = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		type_ = ReceiptType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		mosaic = Mosaic.deserialize(buffer)
+		buffer = buffer[mosaic.size:]
+		target_address = Address.deserialize(buffer)
+		buffer = buffer[target_address.size:]
+
+		instance = LockSecretCreatedFeeReceipt()
+		instance._version = version
+		instance._type_ = type_
+		instance._mosaic = mosaic
+		instance._target_address = target_address
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._type_.serialize()
+		buffer += self._mosaic.serialize()
+		buffer += self._target_address.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'version: 0x{self._version:X}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'mosaic: {self._mosaic.__str__()}, '
+		result += f'target_address: {self._target_address.__str__()}, '
+		result += ')'
+		return result
+
+
+class LockSecretCompletedFeeReceipt:
+	RECEIPT_TYPE: ReceiptType = ReceiptType.LOCK_SECRET_COMPLETED
+	TYPE_HINTS = {
+		'type_': 'enum:ReceiptType',
+		'mosaic': 'struct:Mosaic',
+		'target_address': 'pod:Address'
+	}
+
+	def __init__(self):
+		self._version = 0
+		self._type_ = LockSecretCompletedFeeReceipt.RECEIPT_TYPE
+		self._mosaic = Mosaic()
+		self._target_address = Address()
+
+	def sort(self) -> None:
+		self._mosaic.sort()
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def type_(self) -> ReceiptType:
+		return self._type_
+
+	@property
+	def mosaic(self) -> Mosaic:
+		return self._mosaic
+
+	@property
+	def target_address(self) -> Address:
+		return self._target_address
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@type_.setter
+	def type_(self, value: ReceiptType):
+		self._type_ = value
+
+	@mosaic.setter
+	def mosaic(self, value: Mosaic):
+		self._mosaic = value
+
+	@target_address.setter
+	def target_address(self, value: Address):
+		self._target_address = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 2
+		size += self.type_.size
+		size += self.mosaic.size
+		size += self.target_address.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> LockSecretCompletedFeeReceipt:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		version = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		type_ = ReceiptType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		mosaic = Mosaic.deserialize(buffer)
+		buffer = buffer[mosaic.size:]
+		target_address = Address.deserialize(buffer)
+		buffer = buffer[target_address.size:]
+
+		instance = LockSecretCompletedFeeReceipt()
+		instance._version = version
+		instance._type_ = type_
+		instance._mosaic = mosaic
+		instance._target_address = target_address
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._type_.serialize()
+		buffer += self._mosaic.serialize()
+		buffer += self._target_address.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'version: 0x{self._version:X}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'mosaic: {self._mosaic.__str__()}, '
+		result += f'target_address: {self._target_address.__str__()}, '
+		result += ')'
+		return result
+
+
+class LockSecretExpiredFeeReceipt:
+	RECEIPT_TYPE: ReceiptType = ReceiptType.LOCK_SECRET_EXPIRED
+	TYPE_HINTS = {
+		'type_': 'enum:ReceiptType',
+		'mosaic': 'struct:Mosaic',
+		'target_address': 'pod:Address'
+	}
+
+	def __init__(self):
+		self._version = 0
+		self._type_ = LockSecretExpiredFeeReceipt.RECEIPT_TYPE
+		self._mosaic = Mosaic()
+		self._target_address = Address()
+
+	def sort(self) -> None:
+		self._mosaic.sort()
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def type_(self) -> ReceiptType:
+		return self._type_
+
+	@property
+	def mosaic(self) -> Mosaic:
+		return self._mosaic
+
+	@property
+	def target_address(self) -> Address:
+		return self._target_address
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@type_.setter
+	def type_(self, value: ReceiptType):
+		self._type_ = value
+
+	@mosaic.setter
+	def mosaic(self, value: Mosaic):
+		self._mosaic = value
+
+	@target_address.setter
+	def target_address(self, value: Address):
+		self._target_address = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 2
+		size += self.type_.size
+		size += self.mosaic.size
+		size += self.target_address.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> LockSecretExpiredFeeReceipt:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		version = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		type_ = ReceiptType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		mosaic = Mosaic.deserialize(buffer)
+		buffer = buffer[mosaic.size:]
+		target_address = Address.deserialize(buffer)
+		buffer = buffer[target_address.size:]
+
+		instance = LockSecretExpiredFeeReceipt()
+		instance._version = version
+		instance._type_ = type_
+		instance._mosaic = mosaic
+		instance._target_address = target_address
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._type_.serialize()
+		buffer += self._mosaic.serialize()
+		buffer += self._target_address.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'version: 0x{self._version:X}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'mosaic: {self._mosaic.__str__()}, '
+		result += f'target_address: {self._target_address.__str__()}, '
+		result += ')'
+		return result
+
+
+class MosaicExpiredReceipt:
+	RECEIPT_TYPE: ReceiptType = ReceiptType.MOSAIC_EXPIRED
+	TYPE_HINTS = {
+		'type_': 'enum:ReceiptType',
+		'artifact_id': 'pod:MosaicId'
+	}
+
+	def __init__(self):
+		self._version = 0
+		self._type_ = MosaicExpiredReceipt.RECEIPT_TYPE
+		self._artifact_id = MosaicId()
+
+	def sort(self) -> None:
+		pass
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def type_(self) -> ReceiptType:
+		return self._type_
+
+	@property
+	def artifact_id(self) -> MosaicId:
+		return self._artifact_id
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@type_.setter
+	def type_(self, value: ReceiptType):
+		self._type_ = value
+
+	@artifact_id.setter
+	def artifact_id(self, value: MosaicId):
+		self._artifact_id = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 2
+		size += self.type_.size
+		size += self.artifact_id.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> MosaicExpiredReceipt:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		version = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		type_ = ReceiptType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		artifact_id = MosaicId.deserialize(buffer)
+		buffer = buffer[artifact_id.size:]
+
+		instance = MosaicExpiredReceipt()
+		instance._version = version
+		instance._type_ = type_
+		instance._artifact_id = artifact_id
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._type_.serialize()
+		buffer += self._artifact_id.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'version: 0x{self._version:X}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'artifact_id: {self._artifact_id.__str__()}, '
+		result += ')'
+		return result
+
+
+class MosaicRentalFeeReceipt:
+	RECEIPT_TYPE: ReceiptType = ReceiptType.MOSAIC_RENTAL_FEE
+	TYPE_HINTS = {
+		'type_': 'enum:ReceiptType',
+		'mosaic': 'struct:Mosaic',
+		'sender_address': 'pod:Address',
+		'recipient_address': 'pod:Address'
+	}
+
+	def __init__(self):
+		self._version = 0
+		self._type_ = MosaicRentalFeeReceipt.RECEIPT_TYPE
+		self._mosaic = Mosaic()
+		self._sender_address = Address()
+		self._recipient_address = Address()
+
+	def sort(self) -> None:
+		self._mosaic.sort()
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def type_(self) -> ReceiptType:
+		return self._type_
+
+	@property
+	def mosaic(self) -> Mosaic:
+		return self._mosaic
+
+	@property
+	def sender_address(self) -> Address:
+		return self._sender_address
+
+	@property
+	def recipient_address(self) -> Address:
+		return self._recipient_address
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@type_.setter
+	def type_(self, value: ReceiptType):
+		self._type_ = value
+
+	@mosaic.setter
+	def mosaic(self, value: Mosaic):
+		self._mosaic = value
+
+	@sender_address.setter
+	def sender_address(self, value: Address):
+		self._sender_address = value
+
+	@recipient_address.setter
+	def recipient_address(self, value: Address):
+		self._recipient_address = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 2
+		size += self.type_.size
+		size += self.mosaic.size
+		size += self.sender_address.size
+		size += self.recipient_address.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> MosaicRentalFeeReceipt:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		version = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		type_ = ReceiptType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		mosaic = Mosaic.deserialize(buffer)
+		buffer = buffer[mosaic.size:]
+		sender_address = Address.deserialize(buffer)
+		buffer = buffer[sender_address.size:]
+		recipient_address = Address.deserialize(buffer)
+		buffer = buffer[recipient_address.size:]
+
+		instance = MosaicRentalFeeReceipt()
+		instance._version = version
+		instance._type_ = type_
+		instance._mosaic = mosaic
+		instance._sender_address = sender_address
+		instance._recipient_address = recipient_address
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._type_.serialize()
+		buffer += self._mosaic.serialize()
+		buffer += self._sender_address.serialize()
+		buffer += self._recipient_address.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'version: 0x{self._version:X}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'mosaic: {self._mosaic.__str__()}, '
+		result += f'sender_address: {self._sender_address.__str__()}, '
+		result += f'recipient_address: {self._recipient_address.__str__()}, '
+		result += ')'
+		return result
+
+
+class NamespaceId(BaseValue):
+	SIZE = 8
+
+	def __init__(self, namespace_id: int = 0):
+		super().__init__(self.SIZE, namespace_id, NamespaceId)
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> NamespaceId:
+		buffer = memoryview(payload)
+		return NamespaceId(int.from_bytes(buffer[:8], byteorder='little', signed=False))
+
+	def serialize(self) -> bytes:
+		return self.value.to_bytes(8, byteorder='little', signed=False)
+
+
+class NamespaceRegistrationType(Enum):
+	ROOT = 0
+	CHILD = 1
+
+	@property
+	def size(self) -> int:
+		return 1
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> NamespaceRegistrationType:
+		buffer = memoryview(payload)
+		return NamespaceRegistrationType(int.from_bytes(buffer[:1], byteorder='little', signed=False))
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.value.to_bytes(1, byteorder='little', signed=False)
+		return buffer
+
+
+class AliasAction(Enum):
+	UNLINK = 0
+	LINK = 1
+
+	@property
+	def size(self) -> int:
+		return 1
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> AliasAction:
+		buffer = memoryview(payload)
+		return AliasAction(int.from_bytes(buffer[:1], byteorder='little', signed=False))
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.value.to_bytes(1, byteorder='little', signed=False)
+		return buffer
+
+
+class NamespaceExpiredReceipt:
+	RECEIPT_TYPE: ReceiptType = ReceiptType.NAMESPACE_EXPIRED
+	TYPE_HINTS = {
+		'type_': 'enum:ReceiptType',
+		'artifact_id': 'pod:NamespaceId'
+	}
+
+	def __init__(self):
+		self._version = 0
+		self._type_ = NamespaceExpiredReceipt.RECEIPT_TYPE
+		self._artifact_id = NamespaceId()
+
+	def sort(self) -> None:
+		pass
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def type_(self) -> ReceiptType:
+		return self._type_
+
+	@property
+	def artifact_id(self) -> NamespaceId:
+		return self._artifact_id
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@type_.setter
+	def type_(self, value: ReceiptType):
+		self._type_ = value
+
+	@artifact_id.setter
+	def artifact_id(self, value: NamespaceId):
+		self._artifact_id = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 2
+		size += self.type_.size
+		size += self.artifact_id.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> NamespaceExpiredReceipt:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		version = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		type_ = ReceiptType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		artifact_id = NamespaceId.deserialize(buffer)
+		buffer = buffer[artifact_id.size:]
+
+		instance = NamespaceExpiredReceipt()
+		instance._version = version
+		instance._type_ = type_
+		instance._artifact_id = artifact_id
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._type_.serialize()
+		buffer += self._artifact_id.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'version: 0x{self._version:X}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'artifact_id: {self._artifact_id.__str__()}, '
+		result += ')'
+		return result
+
+
+class NamespaceDeletedReceipt:
+	RECEIPT_TYPE: ReceiptType = ReceiptType.NAMESPACE_DELETED
+	TYPE_HINTS = {
+		'type_': 'enum:ReceiptType',
+		'artifact_id': 'pod:NamespaceId'
+	}
+
+	def __init__(self):
+		self._version = 0
+		self._type_ = NamespaceDeletedReceipt.RECEIPT_TYPE
+		self._artifact_id = NamespaceId()
+
+	def sort(self) -> None:
+		pass
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def type_(self) -> ReceiptType:
+		return self._type_
+
+	@property
+	def artifact_id(self) -> NamespaceId:
+		return self._artifact_id
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@type_.setter
+	def type_(self, value: ReceiptType):
+		self._type_ = value
+
+	@artifact_id.setter
+	def artifact_id(self, value: NamespaceId):
+		self._artifact_id = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 2
+		size += self.type_.size
+		size += self.artifact_id.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> NamespaceDeletedReceipt:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		version = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		type_ = ReceiptType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		artifact_id = NamespaceId.deserialize(buffer)
+		buffer = buffer[artifact_id.size:]
+
+		instance = NamespaceDeletedReceipt()
+		instance._version = version
+		instance._type_ = type_
+		instance._artifact_id = artifact_id
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._type_.serialize()
+		buffer += self._artifact_id.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'version: 0x{self._version:X}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'artifact_id: {self._artifact_id.__str__()}, '
+		result += ')'
+		return result
+
+
+class NamespaceRentalFeeReceipt:
+	RECEIPT_TYPE: ReceiptType = ReceiptType.NAMESPACE_RENTAL_FEE
+	TYPE_HINTS = {
+		'type_': 'enum:ReceiptType',
+		'mosaic': 'struct:Mosaic',
+		'sender_address': 'pod:Address',
+		'recipient_address': 'pod:Address'
+	}
+
+	def __init__(self):
+		self._version = 0
+		self._type_ = NamespaceRentalFeeReceipt.RECEIPT_TYPE
+		self._mosaic = Mosaic()
+		self._sender_address = Address()
+		self._recipient_address = Address()
+
+	def sort(self) -> None:
+		self._mosaic.sort()
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def type_(self) -> ReceiptType:
+		return self._type_
+
+	@property
+	def mosaic(self) -> Mosaic:
+		return self._mosaic
+
+	@property
+	def sender_address(self) -> Address:
+		return self._sender_address
+
+	@property
+	def recipient_address(self) -> Address:
+		return self._recipient_address
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@type_.setter
+	def type_(self, value: ReceiptType):
+		self._type_ = value
+
+	@mosaic.setter
+	def mosaic(self, value: Mosaic):
+		self._mosaic = value
+
+	@sender_address.setter
+	def sender_address(self, value: Address):
+		self._sender_address = value
+
+	@recipient_address.setter
+	def recipient_address(self, value: Address):
+		self._recipient_address = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 2
+		size += self.type_.size
+		size += self.mosaic.size
+		size += self.sender_address.size
+		size += self.recipient_address.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> NamespaceRentalFeeReceipt:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		version = int.from_bytes(buffer[:2], byteorder='little', signed=False)
+		buffer = buffer[2:]
+		type_ = ReceiptType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		mosaic = Mosaic.deserialize(buffer)
+		buffer = buffer[mosaic.size:]
+		sender_address = Address.deserialize(buffer)
+		buffer = buffer[sender_address.size:]
+		recipient_address = Address.deserialize(buffer)
+		buffer = buffer[recipient_address.size:]
+
+		instance = NamespaceRentalFeeReceipt()
+		instance._version = version
+		instance._type_ = type_
+		instance._mosaic = mosaic
+		instance._sender_address = sender_address
+		instance._recipient_address = recipient_address
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(2, byteorder='little', signed=False)
+		buffer += self._type_.serialize()
+		buffer += self._mosaic.serialize()
+		buffer += self._sender_address.serialize()
+		buffer += self._recipient_address.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'version: 0x{self._version:X}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'mosaic: {self._mosaic.__str__()}, '
+		result += f'sender_address: {self._sender_address.__str__()}, '
+		result += f'recipient_address: {self._recipient_address.__str__()}, '
+		result += ')'
+		return result
+
+
+class ReceiptSource:
+	TYPE_HINTS = {
+	}
+
+	def __init__(self):
+		self._primary_id = 0
+		self._secondary_id = 0
+
+	def sort(self) -> None:
+		pass
+
+	@property
+	def primary_id(self) -> int:
+		return self._primary_id
+
+	@property
+	def secondary_id(self) -> int:
+		return self._secondary_id
+
+	@primary_id.setter
+	def primary_id(self, value: int):
+		self._primary_id = value
+
+	@secondary_id.setter
+	def secondary_id(self, value: int):
+		self._secondary_id = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 4
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> ReceiptSource:
+		buffer = memoryview(payload)
+		primary_id = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		secondary_id = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+
+		instance = ReceiptSource()
+		instance._primary_id = primary_id
+		instance._secondary_id = secondary_id
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self._primary_id.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._secondary_id.to_bytes(4, byteorder='little', signed=False)
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'primary_id: 0x{self._primary_id:X}, '
+		result += f'secondary_id: 0x{self._secondary_id:X}, '
+		result += ')'
+		return result
+
+
+class AddressResolutionEntry:
+	TYPE_HINTS = {
+		'source': 'struct:ReceiptSource',
+		'resolved_value': 'pod:Address'
+	}
+
+	def __init__(self):
+		self._source = ReceiptSource()
+		self._resolved_value = Address()
+
+	def sort(self) -> None:
+		self._source.sort()
+
+	@property
+	def source(self) -> ReceiptSource:
+		return self._source
+
+	@property
+	def resolved_value(self) -> Address:
+		return self._resolved_value
+
+	@source.setter
+	def source(self, value: ReceiptSource):
+		self._source = value
+
+	@resolved_value.setter
+	def resolved_value(self, value: Address):
+		self._resolved_value = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += self.source.size
+		size += self.resolved_value.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> AddressResolutionEntry:
+		buffer = memoryview(payload)
+		source = ReceiptSource.deserialize(buffer)
+		buffer = buffer[source.size:]
+		resolved_value = Address.deserialize(buffer)
+		buffer = buffer[resolved_value.size:]
+
+		instance = AddressResolutionEntry()
+		instance._source = source
+		instance._resolved_value = resolved_value
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self._source.serialize()
+		buffer += self._resolved_value.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'source: {self._source.__str__()}, '
+		result += f'resolved_value: {self._resolved_value.__str__()}, '
+		result += ')'
+		return result
+
+
+class AddressResolutionStatement:
+	TYPE_HINTS = {
+		'unresolved': 'pod:UnresolvedAddress',
+		'resolution_entries': 'array[AddressResolutionEntry]'
+	}
+
+	def __init__(self):
+		self._unresolved = UnresolvedAddress()
+		self._resolution_entries = []
+
+	def sort(self) -> None:
+		pass
+
+	@property
+	def unresolved(self) -> UnresolvedAddress:
+		return self._unresolved
+
+	@property
+	def resolution_entries(self) -> List[AddressResolutionEntry]:
+		return self._resolution_entries
+
+	@unresolved.setter
+	def unresolved(self, value: UnresolvedAddress):
+		self._unresolved = value
+
+	@resolution_entries.setter
+	def resolution_entries(self, value: List[AddressResolutionEntry]):
+		self._resolution_entries = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += self.unresolved.size
+		size += 4
+		size += ArrayHelpers.size(self.resolution_entries)
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> AddressResolutionStatement:
+		buffer = memoryview(payload)
+		unresolved = UnresolvedAddress.deserialize(buffer)
+		buffer = buffer[unresolved.size:]
+		resolution_entries_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		resolution_entries = ArrayHelpers.read_array_count(buffer, AddressResolutionEntry, resolution_entries_count)
+		buffer = buffer[ArrayHelpers.size(resolution_entries):]
+
+		instance = AddressResolutionStatement()
+		instance._unresolved = unresolved
+		instance._resolution_entries = resolution_entries
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self._unresolved.serialize()
+		buffer += len(self._resolution_entries).to_bytes(4, byteorder='little', signed=False)  # resolution_entries_count
+		buffer += ArrayHelpers.write_array(self._resolution_entries)
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'unresolved: {self._unresolved.__str__()}, '
+		result += f'resolution_entries: {list(map(str, self._resolution_entries))}, '
+		result += ')'
+		return result
+
+
+class MosaicResolutionEntry:
+	TYPE_HINTS = {
+		'source': 'struct:ReceiptSource',
+		'resolved_value': 'pod:MosaicId'
+	}
+
+	def __init__(self):
+		self._source = ReceiptSource()
+		self._resolved_value = MosaicId()
+
+	def sort(self) -> None:
+		self._source.sort()
+
+	@property
+	def source(self) -> ReceiptSource:
+		return self._source
+
+	@property
+	def resolved_value(self) -> MosaicId:
+		return self._resolved_value
+
+	@source.setter
+	def source(self, value: ReceiptSource):
+		self._source = value
+
+	@resolved_value.setter
+	def resolved_value(self, value: MosaicId):
+		self._resolved_value = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += self.source.size
+		size += self.resolved_value.size
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> MosaicResolutionEntry:
+		buffer = memoryview(payload)
+		source = ReceiptSource.deserialize(buffer)
+		buffer = buffer[source.size:]
+		resolved_value = MosaicId.deserialize(buffer)
+		buffer = buffer[resolved_value.size:]
+
+		instance = MosaicResolutionEntry()
+		instance._source = source
+		instance._resolved_value = resolved_value
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self._source.serialize()
+		buffer += self._resolved_value.serialize()
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'source: {self._source.__str__()}, '
+		result += f'resolved_value: {self._resolved_value.__str__()}, '
+		result += ')'
+		return result
+
+
+class MosaicResolutionStatement:
+	TYPE_HINTS = {
+		'unresolved': 'pod:UnresolvedMosaicId',
+		'resolution_entries': 'array[MosaicResolutionEntry]'
+	}
+
+	def __init__(self):
+		self._unresolved = UnresolvedMosaicId()
+		self._resolution_entries = []
+
+	def sort(self) -> None:
+		pass
+
+	@property
+	def unresolved(self) -> UnresolvedMosaicId:
+		return self._unresolved
+
+	@property
+	def resolution_entries(self) -> List[MosaicResolutionEntry]:
+		return self._resolution_entries
+
+	@unresolved.setter
+	def unresolved(self, value: UnresolvedMosaicId):
+		self._unresolved = value
+
+	@resolution_entries.setter
+	def resolution_entries(self, value: List[MosaicResolutionEntry]):
+		self._resolution_entries = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += self.unresolved.size
+		size += 4
+		size += ArrayHelpers.size(self.resolution_entries)
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> MosaicResolutionStatement:
+		buffer = memoryview(payload)
+		unresolved = UnresolvedMosaicId.deserialize(buffer)
+		buffer = buffer[unresolved.size:]
+		resolution_entries_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		resolution_entries = ArrayHelpers.read_array_count(buffer, MosaicResolutionEntry, resolution_entries_count)
+		buffer = buffer[ArrayHelpers.size(resolution_entries):]
+
+		instance = MosaicResolutionStatement()
+		instance._unresolved = unresolved
+		instance._resolution_entries = resolution_entries
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self._unresolved.serialize()
+		buffer += len(self._resolution_entries).to_bytes(4, byteorder='little', signed=False)  # resolution_entries_count
+		buffer += ArrayHelpers.write_array(self._resolution_entries)
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'unresolved: {self._unresolved.__str__()}, '
+		result += f'resolution_entries: {list(map(str, self._resolution_entries))}, '
+		result += ')'
+		return result
+
+
+class TransactionStatement:
+	TYPE_HINTS = {
+		'receipts': 'array[Receipt]'
+	}
+
+	def __init__(self):
+		self._primary_id = 0
+		self._secondary_id = 0
+		self._receipts = []
+
+	def sort(self) -> None:
+		pass
+
+	@property
+	def primary_id(self) -> int:
+		return self._primary_id
+
+	@property
+	def secondary_id(self) -> int:
+		return self._secondary_id
+
+	@property
+	def receipts(self) -> List[Receipt]:
+		return self._receipts
+
+	@primary_id.setter
+	def primary_id(self, value: int):
+		self._primary_id = value
+
+	@secondary_id.setter
+	def secondary_id(self, value: int):
+		self._secondary_id = value
+
+	@receipts.setter
+	def receipts(self, value: List[Receipt]):
+		self._receipts = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 4
+		size += 4
+		size += ArrayHelpers.size(self.receipts)
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> TransactionStatement:
+		buffer = memoryview(payload)
+		primary_id = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		secondary_id = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		receipt_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		receipts = ArrayHelpers.read_array_count(buffer, ReceiptFactory, receipt_count)
+		buffer = buffer[ArrayHelpers.size(receipts):]
+
+		instance = TransactionStatement()
+		instance._primary_id = primary_id
+		instance._secondary_id = secondary_id
+		instance._receipts = receipts
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self._primary_id.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._secondary_id.to_bytes(4, byteorder='little', signed=False)
+		buffer += len(self._receipts).to_bytes(4, byteorder='little', signed=False)  # receipt_count
+		buffer += ArrayHelpers.write_array(self._receipts)
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'primary_id: 0x{self._primary_id:X}, '
+		result += f'secondary_id: 0x{self._secondary_id:X}, '
+		result += f'receipts: {list(map(str, self._receipts))}, '
+		result += ')'
+		return result
+
+
+class BlockStatement:
+	TYPE_HINTS = {
+		'transaction_statements': 'array[TransactionStatement]',
+		'address_resolution_statements': 'array[AddressResolutionStatement]',
+		'mosaic_resolution_statements': 'array[MosaicResolutionStatement]'
+	}
+
+	def __init__(self):
+		self._transaction_statements = []
+		self._address_resolution_statements = []
+		self._mosaic_resolution_statements = []
+
+	def sort(self) -> None:
+		pass
+
+	@property
+	def transaction_statements(self) -> List[TransactionStatement]:
+		return self._transaction_statements
+
+	@property
+	def address_resolution_statements(self) -> List[AddressResolutionStatement]:
+		return self._address_resolution_statements
+
+	@property
+	def mosaic_resolution_statements(self) -> List[MosaicResolutionStatement]:
+		return self._mosaic_resolution_statements
+
+	@transaction_statements.setter
+	def transaction_statements(self, value: List[TransactionStatement]):
+		self._transaction_statements = value
+
+	@address_resolution_statements.setter
+	def address_resolution_statements(self, value: List[AddressResolutionStatement]):
+		self._address_resolution_statements = value
+
+	@mosaic_resolution_statements.setter
+	def mosaic_resolution_statements(self, value: List[MosaicResolutionStatement]):
+		self._mosaic_resolution_statements = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += ArrayHelpers.size(self.transaction_statements)
+		size += 4
+		size += ArrayHelpers.size(self.address_resolution_statements)
+		size += 4
+		size += ArrayHelpers.size(self.mosaic_resolution_statements)
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> BlockStatement:
+		buffer = memoryview(payload)
+		transaction_statement_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		transaction_statements = ArrayHelpers.read_array_count(buffer, TransactionStatement, transaction_statement_count)
+		buffer = buffer[ArrayHelpers.size(transaction_statements):]
+		address_resolution_statement_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		address_resolution_statements = ArrayHelpers.read_array_count(buffer, AddressResolutionStatement, address_resolution_statement_count)
+		buffer = buffer[ArrayHelpers.size(address_resolution_statements):]
+		mosaic_resolution_statement_count = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		mosaic_resolution_statements = ArrayHelpers.read_array_count(buffer, MosaicResolutionStatement, mosaic_resolution_statement_count)
+		buffer = buffer[ArrayHelpers.size(mosaic_resolution_statements):]
+
+		instance = BlockStatement()
+		instance._transaction_statements = transaction_statements
+		instance._address_resolution_statements = address_resolution_statements
+		instance._mosaic_resolution_statements = mosaic_resolution_statements
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += len(self._transaction_statements).to_bytes(4, byteorder='little', signed=False)  # transaction_statement_count
+		buffer += ArrayHelpers.write_array(self._transaction_statements)
+		buffer += len(self._address_resolution_statements).to_bytes(4, byteorder='little', signed=False)  # address_resolution_statement_count
+		buffer += ArrayHelpers.write_array(self._address_resolution_statements)
+		buffer += len(self._mosaic_resolution_statements).to_bytes(4, byteorder='little', signed=False)  # mosaic_resolution_statement_count
+		buffer += ArrayHelpers.write_array(self._mosaic_resolution_statements)
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'transaction_statements: {list(map(str, self._transaction_statements))}, '
+		result += f'address_resolution_statements: {list(map(str, self._address_resolution_statements))}, '
+		result += f'mosaic_resolution_statements: {list(map(str, self._mosaic_resolution_statements))}, '
+		result += ')'
+		return result
+
+
+class AccountKeyLinkTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.ACCOUNT_KEY_LINK
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -812,24 +4386,27 @@
 		'linked_public_key': 'pod:PublicKey',
 		'link_action': 'enum:LinkAction'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = AccountKeyLinkTransaction.TRANSACTION_VERSION
+		self._version = AccountKeyLinkTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = AccountKeyLinkTransaction.TRANSACTION_TYPE
+		self._type_ = AccountKeyLinkTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._linked_public_key = PublicKey()
 		self._link_action = LinkAction.UNLINK
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -912,15 +4489,15 @@
 		size += self.fee.size
 		size += self.deadline.size
 		size += self.linked_public_key.size
 		size += self.link_action.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> AccountKeyLinkTransaction:
+	def deserialize(cls, payload: ByteString) -> AccountKeyLinkTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -943,15 +4520,15 @@
 		deadline = Timestamp.deserialize(buffer)
 		buffer = buffer[deadline.size:]
 		linked_public_key = PublicKey.deserialize(buffer)
 		buffer = buffer[linked_public_key.size:]
 		link_action = LinkAction.deserialize(buffer)
 		buffer = buffer[link_action.size:]
 
-		instance = AccountKeyLinkTransaction()
+		instance = AccountKeyLinkTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -986,35 +4563,38 @@
 		result += f'deadline: {self._deadline.__str__()}, '
 		result += f'linked_public_key: {self._linked_public_key.__str__()}, '
 		result += f'link_action: {self._link_action.__str__()}, '
 		result += ')'
 		return result
 
 
-class EmbeddedAccountKeyLinkTransaction:
+class EmbeddedAccountKeyLinkTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.ACCOUNT_KEY_LINK
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'linked_public_key': 'pod:PublicKey',
 		'link_action': 'enum:LinkAction'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedAccountKeyLinkTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedAccountKeyLinkTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedAccountKeyLinkTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedAccountKeyLinkTransactionV1.TRANSACTION_TYPE
 		self._linked_public_key = PublicKey()
 		self._link_action = LinkAction.UNLINK
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -1070,15 +4650,15 @@
 		size += self.network.size
 		size += self.type_.size
 		size += self.linked_public_key.size
 		size += self.link_action.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedAccountKeyLinkTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedAccountKeyLinkTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -1095,15 +4675,15 @@
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		linked_public_key = PublicKey.deserialize(buffer)
 		buffer = buffer[linked_public_key.size:]
 		link_action = LinkAction.deserialize(buffer)
 		buffer = buffer[link_action.size:]
 
-		instance = EmbeddedAccountKeyLinkTransaction()
+		instance = EmbeddedAccountKeyLinkTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._linked_public_key = linked_public_key
 		instance._link_action = link_action
 		return instance
@@ -1129,15 +4709,15 @@
 		result += f'type_: {self._type_.__str__()}, '
 		result += f'linked_public_key: {self._linked_public_key.__str__()}, '
 		result += f'link_action: {self._link_action.__str__()}, '
 		result += ')'
 		return result
 
 
-class NodeKeyLinkTransaction:
+class NodeKeyLinkTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.NODE_KEY_LINK
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -1146,24 +4726,27 @@
 		'linked_public_key': 'pod:PublicKey',
 		'link_action': 'enum:LinkAction'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = NodeKeyLinkTransaction.TRANSACTION_VERSION
+		self._version = NodeKeyLinkTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = NodeKeyLinkTransaction.TRANSACTION_TYPE
+		self._type_ = NodeKeyLinkTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._linked_public_key = PublicKey()
 		self._link_action = LinkAction.UNLINK
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -1246,15 +4829,15 @@
 		size += self.fee.size
 		size += self.deadline.size
 		size += self.linked_public_key.size
 		size += self.link_action.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> NodeKeyLinkTransaction:
+	def deserialize(cls, payload: ByteString) -> NodeKeyLinkTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -1277,15 +4860,15 @@
 		deadline = Timestamp.deserialize(buffer)
 		buffer = buffer[deadline.size:]
 		linked_public_key = PublicKey.deserialize(buffer)
 		buffer = buffer[linked_public_key.size:]
 		link_action = LinkAction.deserialize(buffer)
 		buffer = buffer[link_action.size:]
 
-		instance = NodeKeyLinkTransaction()
+		instance = NodeKeyLinkTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -1320,35 +4903,38 @@
 		result += f'deadline: {self._deadline.__str__()}, '
 		result += f'linked_public_key: {self._linked_public_key.__str__()}, '
 		result += f'link_action: {self._link_action.__str__()}, '
 		result += ')'
 		return result
 
 
-class EmbeddedNodeKeyLinkTransaction:
+class EmbeddedNodeKeyLinkTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.NODE_KEY_LINK
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'linked_public_key': 'pod:PublicKey',
 		'link_action': 'enum:LinkAction'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedNodeKeyLinkTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedNodeKeyLinkTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedNodeKeyLinkTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedNodeKeyLinkTransactionV1.TRANSACTION_TYPE
 		self._linked_public_key = PublicKey()
 		self._link_action = LinkAction.UNLINK
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -1404,15 +4990,15 @@
 		size += self.network.size
 		size += self.type_.size
 		size += self.linked_public_key.size
 		size += self.link_action.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedNodeKeyLinkTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedNodeKeyLinkTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -1429,15 +5015,15 @@
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		linked_public_key = PublicKey.deserialize(buffer)
 		buffer = buffer[linked_public_key.size:]
 		link_action = LinkAction.deserialize(buffer)
 		buffer = buffer[link_action.size:]
 
-		instance = EmbeddedNodeKeyLinkTransaction()
+		instance = EmbeddedNodeKeyLinkTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._linked_public_key = linked_public_key
 		instance._link_action = link_action
 		return instance
@@ -1474,14 +5060,17 @@
 	}
 
 	def __init__(self):
 		self._version = 0
 		self._signer_public_key = PublicKey()
 		self._signature = Signature()
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def version(self) -> int:
 		return self._version
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -1551,14 +5140,17 @@
 
 	def __init__(self):
 		self._version = 0
 		self._signer_public_key = PublicKey()
 		self._signature = Signature()
 		self._parent_hash = Hash256()
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def version(self) -> int:
 		return self._version
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -1629,15 +5221,15 @@
 		result += f'signer_public_key: {self._signer_public_key.__str__()}, '
 		result += f'signature: {self._signature.__str__()}, '
 		result += f'parent_hash: {self._parent_hash.__str__()}, '
 		result += ')'
 		return result
 
 
-class AggregateCompleteTransaction:
+class AggregateCompleteTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.AGGREGATE_COMPLETE
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -1647,26 +5239,29 @@
 		'transactions': 'array[EmbeddedTransaction]',
 		'cosignatures': 'array[Cosignature]'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = AggregateCompleteTransaction.TRANSACTION_VERSION
+		self._version = AggregateCompleteTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = AggregateCompleteTransaction.TRANSACTION_TYPE
+		self._type_ = AggregateCompleteTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._transactions_hash = Hash256()
 		self._transactions = []
 		self._cosignatures = []
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._aggregate_transaction_header_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -1760,15 +5355,15 @@
 		size += 4
 		size += 4
 		size += ArrayHelpers.size(self.transactions, 8, skip_last_element_padding=False)
 		size += ArrayHelpers.size(self.cosignatures)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> AggregateCompleteTransaction:
+	def deserialize(cls, payload: ByteString) -> AggregateCompleteTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -1798,15 +5393,15 @@
 		buffer = buffer[4:]
 		assert aggregate_transaction_header_reserved_1 == 0, f'Invalid value of reserved field ({aggregate_transaction_header_reserved_1})'
 		transactions = ArrayHelpers.read_variable_size_elements(buffer[:payload_size], EmbeddedTransactionFactory, 8, skip_last_element_padding=False)
 		buffer = buffer[payload_size:]
 		cosignatures = ArrayHelpers.read_array(buffer, Cosignature)
 		buffer = buffer[ArrayHelpers.size(cosignatures):]
 
-		instance = AggregateCompleteTransaction()
+		instance = AggregateCompleteTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -1846,15 +5441,235 @@
 		result += f'transactions_hash: {self._transactions_hash.__str__()}, '
 		result += f'transactions: {list(map(str, self._transactions))}, '
 		result += f'cosignatures: {list(map(str, self._cosignatures))}, '
 		result += ')'
 		return result
 
 
-class AggregateBondedTransaction:
+class AggregateCompleteTransactionV2:
+	TRANSACTION_VERSION: int = 2
+	TRANSACTION_TYPE: TransactionType = TransactionType.AGGREGATE_COMPLETE
+	TYPE_HINTS = {
+		'signature': 'pod:Signature',
+		'signer_public_key': 'pod:PublicKey',
+		'network': 'enum:NetworkType',
+		'type_': 'enum:TransactionType',
+		'fee': 'pod:Amount',
+		'deadline': 'pod:Timestamp',
+		'transactions_hash': 'pod:Hash256',
+		'transactions': 'array[EmbeddedTransaction]',
+		'cosignatures': 'array[Cosignature]'
+	}
+
+	def __init__(self):
+		self._signature = Signature()
+		self._signer_public_key = PublicKey()
+		self._version = AggregateCompleteTransactionV2.TRANSACTION_VERSION
+		self._network = NetworkType.MAINNET
+		self._type_ = AggregateCompleteTransactionV2.TRANSACTION_TYPE
+		self._fee = Amount()
+		self._deadline = Timestamp()
+		self._transactions_hash = Hash256()
+		self._transactions = []
+		self._cosignatures = []
+		self._verifiable_entity_header_reserved_1 = 0  # reserved field
+		self._entity_body_reserved_1 = 0  # reserved field
+		self._aggregate_transaction_header_reserved_1 = 0  # reserved field
+
+	def sort(self) -> None:
+		pass
+
+	@property
+	def signature(self) -> Signature:
+		return self._signature
+
+	@property
+	def signer_public_key(self) -> PublicKey:
+		return self._signer_public_key
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def network(self) -> NetworkType:
+		return self._network
+
+	@property
+	def type_(self) -> TransactionType:
+		return self._type_
+
+	@property
+	def fee(self) -> Amount:
+		return self._fee
+
+	@property
+	def deadline(self) -> Timestamp:
+		return self._deadline
+
+	@property
+	def transactions_hash(self) -> Hash256:
+		return self._transactions_hash
+
+	@property
+	def transactions(self) -> List[EmbeddedTransaction]:
+		return self._transactions
+
+	@property
+	def cosignatures(self) -> List[Cosignature]:
+		return self._cosignatures
+
+	@signature.setter
+	def signature(self, value: Signature):
+		self._signature = value
+
+	@signer_public_key.setter
+	def signer_public_key(self, value: PublicKey):
+		self._signer_public_key = value
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@network.setter
+	def network(self, value: NetworkType):
+		self._network = value
+
+	@type_.setter
+	def type_(self, value: TransactionType):
+		self._type_ = value
+
+	@fee.setter
+	def fee(self, value: Amount):
+		self._fee = value
+
+	@deadline.setter
+	def deadline(self, value: Timestamp):
+		self._deadline = value
+
+	@transactions_hash.setter
+	def transactions_hash(self, value: Hash256):
+		self._transactions_hash = value
+
+	@transactions.setter
+	def transactions(self, value: List[EmbeddedTransaction]):
+		self._transactions = value
+
+	@cosignatures.setter
+	def cosignatures(self, value: List[Cosignature]):
+		self._cosignatures = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 4
+		size += self.signature.size
+		size += self.signer_public_key.size
+		size += 4
+		size += 1
+		size += self.network.size
+		size += self.type_.size
+		size += self.fee.size
+		size += self.deadline.size
+		size += self.transactions_hash.size
+		size += 4
+		size += 4
+		size += ArrayHelpers.size(self.transactions, 8, skip_last_element_padding=False)
+		size += ArrayHelpers.size(self.cosignatures)
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> AggregateCompleteTransactionV2:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert verifiable_entity_header_reserved_1 == 0, f'Invalid value of reserved field ({verifiable_entity_header_reserved_1})'
+		signature = Signature.deserialize(buffer)
+		buffer = buffer[signature.size:]
+		signer_public_key = PublicKey.deserialize(buffer)
+		buffer = buffer[signer_public_key.size:]
+		entity_body_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert entity_body_reserved_1 == 0, f'Invalid value of reserved field ({entity_body_reserved_1})'
+		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
+		buffer = buffer[1:]
+		network = NetworkType.deserialize(buffer)
+		buffer = buffer[network.size:]
+		type_ = TransactionType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		fee = Amount.deserialize(buffer)
+		buffer = buffer[fee.size:]
+		deadline = Timestamp.deserialize(buffer)
+		buffer = buffer[deadline.size:]
+		transactions_hash = Hash256.deserialize(buffer)
+		buffer = buffer[transactions_hash.size:]
+		payload_size = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		aggregate_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert aggregate_transaction_header_reserved_1 == 0, f'Invalid value of reserved field ({aggregate_transaction_header_reserved_1})'
+		transactions = ArrayHelpers.read_variable_size_elements(buffer[:payload_size], EmbeddedTransactionFactory, 8, skip_last_element_padding=False)
+		buffer = buffer[payload_size:]
+		cosignatures = ArrayHelpers.read_array(buffer, Cosignature)
+		buffer = buffer[ArrayHelpers.size(cosignatures):]
+
+		instance = AggregateCompleteTransactionV2()
+		instance._signature = signature
+		instance._signer_public_key = signer_public_key
+		instance._version = version
+		instance._network = network
+		instance._type_ = type_
+		instance._fee = fee
+		instance._deadline = deadline
+		instance._transactions_hash = transactions_hash
+		instance._transactions = transactions
+		instance._cosignatures = cosignatures
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._verifiable_entity_header_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._signature.serialize()
+		buffer += self._signer_public_key.serialize()
+		buffer += self._entity_body_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(1, byteorder='little', signed=False)
+		buffer += self._network.serialize()
+		buffer += self._type_.serialize()
+		buffer += self._fee.serialize()
+		buffer += self._deadline.serialize()
+		buffer += self._transactions_hash.serialize()
+		buffer += ArrayHelpers.size(self.transactions, 8, skip_last_element_padding=False).to_bytes(4, byteorder='little', signed=False)  # payload_size
+		buffer += self._aggregate_transaction_header_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += ArrayHelpers.write_variable_size_elements(self._transactions, 8, skip_last_element_padding=False)
+		buffer += ArrayHelpers.write_array(self._cosignatures)
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'signature: {self._signature.__str__()}, '
+		result += f'signer_public_key: {self._signer_public_key.__str__()}, '
+		result += f'version: 0x{self._version:X}, '
+		result += f'network: {self._network.__str__()}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'fee: {self._fee.__str__()}, '
+		result += f'deadline: {self._deadline.__str__()}, '
+		result += f'transactions_hash: {self._transactions_hash.__str__()}, '
+		result += f'transactions: {list(map(str, self._transactions))}, '
+		result += f'cosignatures: {list(map(str, self._cosignatures))}, '
+		result += ')'
+		return result
+
+
+class AggregateBondedTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.AGGREGATE_BONDED
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -1864,26 +5679,29 @@
 		'transactions': 'array[EmbeddedTransaction]',
 		'cosignatures': 'array[Cosignature]'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = AggregateBondedTransaction.TRANSACTION_VERSION
+		self._version = AggregateBondedTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = AggregateBondedTransaction.TRANSACTION_TYPE
+		self._type_ = AggregateBondedTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._transactions_hash = Hash256()
 		self._transactions = []
 		self._cosignatures = []
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._aggregate_transaction_header_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -1977,15 +5795,15 @@
 		size += 4
 		size += 4
 		size += ArrayHelpers.size(self.transactions, 8, skip_last_element_padding=False)
 		size += ArrayHelpers.size(self.cosignatures)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> AggregateBondedTransaction:
+	def deserialize(cls, payload: ByteString) -> AggregateBondedTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -2015,15 +5833,15 @@
 		buffer = buffer[4:]
 		assert aggregate_transaction_header_reserved_1 == 0, f'Invalid value of reserved field ({aggregate_transaction_header_reserved_1})'
 		transactions = ArrayHelpers.read_variable_size_elements(buffer[:payload_size], EmbeddedTransactionFactory, 8, skip_last_element_padding=False)
 		buffer = buffer[payload_size:]
 		cosignatures = ArrayHelpers.read_array(buffer, Cosignature)
 		buffer = buffer[ArrayHelpers.size(cosignatures):]
 
-		instance = AggregateBondedTransaction()
+		instance = AggregateBondedTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -2063,15 +5881,235 @@
 		result += f'transactions_hash: {self._transactions_hash.__str__()}, '
 		result += f'transactions: {list(map(str, self._transactions))}, '
 		result += f'cosignatures: {list(map(str, self._cosignatures))}, '
 		result += ')'
 		return result
 
 
-class VotingKeyLinkTransaction:
+class AggregateBondedTransactionV2:
+	TRANSACTION_VERSION: int = 2
+	TRANSACTION_TYPE: TransactionType = TransactionType.AGGREGATE_BONDED
+	TYPE_HINTS = {
+		'signature': 'pod:Signature',
+		'signer_public_key': 'pod:PublicKey',
+		'network': 'enum:NetworkType',
+		'type_': 'enum:TransactionType',
+		'fee': 'pod:Amount',
+		'deadline': 'pod:Timestamp',
+		'transactions_hash': 'pod:Hash256',
+		'transactions': 'array[EmbeddedTransaction]',
+		'cosignatures': 'array[Cosignature]'
+	}
+
+	def __init__(self):
+		self._signature = Signature()
+		self._signer_public_key = PublicKey()
+		self._version = AggregateBondedTransactionV2.TRANSACTION_VERSION
+		self._network = NetworkType.MAINNET
+		self._type_ = AggregateBondedTransactionV2.TRANSACTION_TYPE
+		self._fee = Amount()
+		self._deadline = Timestamp()
+		self._transactions_hash = Hash256()
+		self._transactions = []
+		self._cosignatures = []
+		self._verifiable_entity_header_reserved_1 = 0  # reserved field
+		self._entity_body_reserved_1 = 0  # reserved field
+		self._aggregate_transaction_header_reserved_1 = 0  # reserved field
+
+	def sort(self) -> None:
+		pass
+
+	@property
+	def signature(self) -> Signature:
+		return self._signature
+
+	@property
+	def signer_public_key(self) -> PublicKey:
+		return self._signer_public_key
+
+	@property
+	def version(self) -> int:
+		return self._version
+
+	@property
+	def network(self) -> NetworkType:
+		return self._network
+
+	@property
+	def type_(self) -> TransactionType:
+		return self._type_
+
+	@property
+	def fee(self) -> Amount:
+		return self._fee
+
+	@property
+	def deadline(self) -> Timestamp:
+		return self._deadline
+
+	@property
+	def transactions_hash(self) -> Hash256:
+		return self._transactions_hash
+
+	@property
+	def transactions(self) -> List[EmbeddedTransaction]:
+		return self._transactions
+
+	@property
+	def cosignatures(self) -> List[Cosignature]:
+		return self._cosignatures
+
+	@signature.setter
+	def signature(self, value: Signature):
+		self._signature = value
+
+	@signer_public_key.setter
+	def signer_public_key(self, value: PublicKey):
+		self._signer_public_key = value
+
+	@version.setter
+	def version(self, value: int):
+		self._version = value
+
+	@network.setter
+	def network(self, value: NetworkType):
+		self._network = value
+
+	@type_.setter
+	def type_(self, value: TransactionType):
+		self._type_ = value
+
+	@fee.setter
+	def fee(self, value: Amount):
+		self._fee = value
+
+	@deadline.setter
+	def deadline(self, value: Timestamp):
+		self._deadline = value
+
+	@transactions_hash.setter
+	def transactions_hash(self, value: Hash256):
+		self._transactions_hash = value
+
+	@transactions.setter
+	def transactions(self, value: List[EmbeddedTransaction]):
+		self._transactions = value
+
+	@cosignatures.setter
+	def cosignatures(self, value: List[Cosignature]):
+		self._cosignatures = value
+
+	@property
+	def size(self) -> int:
+		size = 0
+		size += 4
+		size += 4
+		size += self.signature.size
+		size += self.signer_public_key.size
+		size += 4
+		size += 1
+		size += self.network.size
+		size += self.type_.size
+		size += self.fee.size
+		size += self.deadline.size
+		size += self.transactions_hash.size
+		size += 4
+		size += 4
+		size += ArrayHelpers.size(self.transactions, 8, skip_last_element_padding=False)
+		size += ArrayHelpers.size(self.cosignatures)
+		return size
+
+	@classmethod
+	def deserialize(cls, payload: ByteString) -> AggregateBondedTransactionV2:
+		buffer = memoryview(payload)
+		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		buffer = buffer[:size_ - 4]
+		del size_
+		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert verifiable_entity_header_reserved_1 == 0, f'Invalid value of reserved field ({verifiable_entity_header_reserved_1})'
+		signature = Signature.deserialize(buffer)
+		buffer = buffer[signature.size:]
+		signer_public_key = PublicKey.deserialize(buffer)
+		buffer = buffer[signer_public_key.size:]
+		entity_body_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert entity_body_reserved_1 == 0, f'Invalid value of reserved field ({entity_body_reserved_1})'
+		version = int.from_bytes(buffer[:1], byteorder='little', signed=False)
+		buffer = buffer[1:]
+		network = NetworkType.deserialize(buffer)
+		buffer = buffer[network.size:]
+		type_ = TransactionType.deserialize(buffer)
+		buffer = buffer[type_.size:]
+		fee = Amount.deserialize(buffer)
+		buffer = buffer[fee.size:]
+		deadline = Timestamp.deserialize(buffer)
+		buffer = buffer[deadline.size:]
+		transactions_hash = Hash256.deserialize(buffer)
+		buffer = buffer[transactions_hash.size:]
+		payload_size = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		aggregate_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
+		buffer = buffer[4:]
+		assert aggregate_transaction_header_reserved_1 == 0, f'Invalid value of reserved field ({aggregate_transaction_header_reserved_1})'
+		transactions = ArrayHelpers.read_variable_size_elements(buffer[:payload_size], EmbeddedTransactionFactory, 8, skip_last_element_padding=False)
+		buffer = buffer[payload_size:]
+		cosignatures = ArrayHelpers.read_array(buffer, Cosignature)
+		buffer = buffer[ArrayHelpers.size(cosignatures):]
+
+		instance = AggregateBondedTransactionV2()
+		instance._signature = signature
+		instance._signer_public_key = signer_public_key
+		instance._version = version
+		instance._network = network
+		instance._type_ = type_
+		instance._fee = fee
+		instance._deadline = deadline
+		instance._transactions_hash = transactions_hash
+		instance._transactions = transactions
+		instance._cosignatures = cosignatures
+		return instance
+
+	def serialize(self) -> bytes:
+		buffer = bytes()
+		buffer += self.size.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._verifiable_entity_header_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._signature.serialize()
+		buffer += self._signer_public_key.serialize()
+		buffer += self._entity_body_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += self._version.to_bytes(1, byteorder='little', signed=False)
+		buffer += self._network.serialize()
+		buffer += self._type_.serialize()
+		buffer += self._fee.serialize()
+		buffer += self._deadline.serialize()
+		buffer += self._transactions_hash.serialize()
+		buffer += ArrayHelpers.size(self.transactions, 8, skip_last_element_padding=False).to_bytes(4, byteorder='little', signed=False)  # payload_size
+		buffer += self._aggregate_transaction_header_reserved_1.to_bytes(4, byteorder='little', signed=False)
+		buffer += ArrayHelpers.write_variable_size_elements(self._transactions, 8, skip_last_element_padding=False)
+		buffer += ArrayHelpers.write_array(self._cosignatures)
+		return buffer
+
+	def __str__(self) -> str:
+		result = '('
+		result += f'signature: {self._signature.__str__()}, '
+		result += f'signer_public_key: {self._signer_public_key.__str__()}, '
+		result += f'version: 0x{self._version:X}, '
+		result += f'network: {self._network.__str__()}, '
+		result += f'type_: {self._type_.__str__()}, '
+		result += f'fee: {self._fee.__str__()}, '
+		result += f'deadline: {self._deadline.__str__()}, '
+		result += f'transactions_hash: {self._transactions_hash.__str__()}, '
+		result += f'transactions: {list(map(str, self._transactions))}, '
+		result += f'cosignatures: {list(map(str, self._cosignatures))}, '
+		result += ')'
+		return result
+
+
+class VotingKeyLinkTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.VOTING_KEY_LINK
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -2082,26 +6120,29 @@
 		'end_epoch': 'pod:FinalizationEpoch',
 		'link_action': 'enum:LinkAction'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = VotingKeyLinkTransaction.TRANSACTION_VERSION
+		self._version = VotingKeyLinkTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = VotingKeyLinkTransaction.TRANSACTION_TYPE
+		self._type_ = VotingKeyLinkTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._linked_public_key = VotingPublicKey()
 		self._start_epoch = FinalizationEpoch()
 		self._end_epoch = FinalizationEpoch()
 		self._link_action = LinkAction.UNLINK
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -2202,15 +6243,15 @@
 		size += self.linked_public_key.size
 		size += self.start_epoch.size
 		size += self.end_epoch.size
 		size += self.link_action.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> VotingKeyLinkTransaction:
+	def deserialize(cls, payload: ByteString) -> VotingKeyLinkTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -2237,15 +6278,15 @@
 		start_epoch = FinalizationEpoch.deserialize(buffer)
 		buffer = buffer[start_epoch.size:]
 		end_epoch = FinalizationEpoch.deserialize(buffer)
 		buffer = buffer[end_epoch.size:]
 		link_action = LinkAction.deserialize(buffer)
 		buffer = buffer[link_action.size:]
 
-		instance = VotingKeyLinkTransaction()
+		instance = VotingKeyLinkTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -2286,39 +6327,42 @@
 		result += f'start_epoch: {self._start_epoch.__str__()}, '
 		result += f'end_epoch: {self._end_epoch.__str__()}, '
 		result += f'link_action: {self._link_action.__str__()}, '
 		result += ')'
 		return result
 
 
-class EmbeddedVotingKeyLinkTransaction:
+class EmbeddedVotingKeyLinkTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.VOTING_KEY_LINK
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'linked_public_key': 'pod:VotingPublicKey',
 		'start_epoch': 'pod:FinalizationEpoch',
 		'end_epoch': 'pod:FinalizationEpoch',
 		'link_action': 'enum:LinkAction'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedVotingKeyLinkTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedVotingKeyLinkTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedVotingKeyLinkTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedVotingKeyLinkTransactionV1.TRANSACTION_TYPE
 		self._linked_public_key = VotingPublicKey()
 		self._start_epoch = FinalizationEpoch()
 		self._end_epoch = FinalizationEpoch()
 		self._link_action = LinkAction.UNLINK
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -2392,15 +6436,15 @@
 		size += self.linked_public_key.size
 		size += self.start_epoch.size
 		size += self.end_epoch.size
 		size += self.link_action.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedVotingKeyLinkTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedVotingKeyLinkTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -2421,15 +6465,15 @@
 		start_epoch = FinalizationEpoch.deserialize(buffer)
 		buffer = buffer[start_epoch.size:]
 		end_epoch = FinalizationEpoch.deserialize(buffer)
 		buffer = buffer[end_epoch.size:]
 		link_action = LinkAction.deserialize(buffer)
 		buffer = buffer[link_action.size:]
 
-		instance = EmbeddedVotingKeyLinkTransaction()
+		instance = EmbeddedVotingKeyLinkTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._linked_public_key = linked_public_key
 		instance._start_epoch = start_epoch
 		instance._end_epoch = end_epoch
@@ -2461,15 +6505,15 @@
 		result += f'start_epoch: {self._start_epoch.__str__()}, '
 		result += f'end_epoch: {self._end_epoch.__str__()}, '
 		result += f'link_action: {self._link_action.__str__()}, '
 		result += ')'
 		return result
 
 
-class VrfKeyLinkTransaction:
+class VrfKeyLinkTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.VRF_KEY_LINK
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -2478,24 +6522,27 @@
 		'linked_public_key': 'pod:PublicKey',
 		'link_action': 'enum:LinkAction'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = VrfKeyLinkTransaction.TRANSACTION_VERSION
+		self._version = VrfKeyLinkTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = VrfKeyLinkTransaction.TRANSACTION_TYPE
+		self._type_ = VrfKeyLinkTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._linked_public_key = PublicKey()
 		self._link_action = LinkAction.UNLINK
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -2578,15 +6625,15 @@
 		size += self.fee.size
 		size += self.deadline.size
 		size += self.linked_public_key.size
 		size += self.link_action.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> VrfKeyLinkTransaction:
+	def deserialize(cls, payload: ByteString) -> VrfKeyLinkTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -2609,15 +6656,15 @@
 		deadline = Timestamp.deserialize(buffer)
 		buffer = buffer[deadline.size:]
 		linked_public_key = PublicKey.deserialize(buffer)
 		buffer = buffer[linked_public_key.size:]
 		link_action = LinkAction.deserialize(buffer)
 		buffer = buffer[link_action.size:]
 
-		instance = VrfKeyLinkTransaction()
+		instance = VrfKeyLinkTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -2652,35 +6699,38 @@
 		result += f'deadline: {self._deadline.__str__()}, '
 		result += f'linked_public_key: {self._linked_public_key.__str__()}, '
 		result += f'link_action: {self._link_action.__str__()}, '
 		result += ')'
 		return result
 
 
-class EmbeddedVrfKeyLinkTransaction:
+class EmbeddedVrfKeyLinkTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.VRF_KEY_LINK
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'linked_public_key': 'pod:PublicKey',
 		'link_action': 'enum:LinkAction'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedVrfKeyLinkTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedVrfKeyLinkTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedVrfKeyLinkTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedVrfKeyLinkTransactionV1.TRANSACTION_TYPE
 		self._linked_public_key = PublicKey()
 		self._link_action = LinkAction.UNLINK
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -2736,15 +6786,15 @@
 		size += self.network.size
 		size += self.type_.size
 		size += self.linked_public_key.size
 		size += self.link_action.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedVrfKeyLinkTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedVrfKeyLinkTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -2761,15 +6811,15 @@
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		linked_public_key = PublicKey.deserialize(buffer)
 		buffer = buffer[linked_public_key.size:]
 		link_action = LinkAction.deserialize(buffer)
 		buffer = buffer[link_action.size:]
 
-		instance = EmbeddedVrfKeyLinkTransaction()
+		instance = EmbeddedVrfKeyLinkTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._linked_public_key = linked_public_key
 		instance._link_action = link_action
 		return instance
@@ -2795,15 +6845,15 @@
 		result += f'type_: {self._type_.__str__()}, '
 		result += f'linked_public_key: {self._linked_public_key.__str__()}, '
 		result += f'link_action: {self._link_action.__str__()}, '
 		result += ')'
 		return result
 
 
-class HashLockTransaction:
+class HashLockTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.HASH_LOCK
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -2813,25 +6863,28 @@
 		'duration': 'pod:BlockDuration',
 		'hash': 'pod:Hash256'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = HashLockTransaction.TRANSACTION_VERSION
+		self._version = HashLockTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = HashLockTransaction.TRANSACTION_TYPE
+		self._type_ = HashLockTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._mosaic = UnresolvedMosaic()
 		self._duration = BlockDuration()
 		self._hash = Hash256()
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		self._mosaic.sort()
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -2923,15 +6976,15 @@
 		size += self.deadline.size
 		size += self.mosaic.size
 		size += self.duration.size
 		size += self.hash.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> HashLockTransaction:
+	def deserialize(cls, payload: ByteString) -> HashLockTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -2956,15 +7009,15 @@
 		mosaic = UnresolvedMosaic.deserialize(buffer)
 		buffer = buffer[mosaic.size:]
 		duration = BlockDuration.deserialize(buffer)
 		buffer = buffer[duration.size:]
 		hash = Hash256.deserialize(buffer)
 		buffer = buffer[hash.size:]
 
-		instance = HashLockTransaction()
+		instance = HashLockTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -3002,37 +7055,40 @@
 		result += f'mosaic: {self._mosaic.__str__()}, '
 		result += f'duration: {self._duration.__str__()}, '
 		result += f'hash: {self._hash.__str__()}, '
 		result += ')'
 		return result
 
 
-class EmbeddedHashLockTransaction:
+class EmbeddedHashLockTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.HASH_LOCK
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'mosaic': 'struct:UnresolvedMosaic',
 		'duration': 'pod:BlockDuration',
 		'hash': 'pod:Hash256'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedHashLockTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedHashLockTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedHashLockTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedHashLockTransactionV1.TRANSACTION_TYPE
 		self._mosaic = UnresolvedMosaic()
 		self._duration = BlockDuration()
 		self._hash = Hash256()
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		self._mosaic.sort()
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -3097,15 +7153,15 @@
 		size += self.type_.size
 		size += self.mosaic.size
 		size += self.duration.size
 		size += self.hash.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedHashLockTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedHashLockTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -3124,15 +7180,15 @@
 		mosaic = UnresolvedMosaic.deserialize(buffer)
 		buffer = buffer[mosaic.size:]
 		duration = BlockDuration.deserialize(buffer)
 		buffer = buffer[duration.size:]
 		hash = Hash256.deserialize(buffer)
 		buffer = buffer[hash.size:]
 
-		instance = EmbeddedHashLockTransaction()
+		instance = EmbeddedHashLockTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._mosaic = mosaic
 		instance._duration = duration
 		instance._hash = hash
@@ -3181,15 +7237,15 @@
 
 	def serialize(self) -> bytes:
 		buffer = bytes()
 		buffer += self.value.to_bytes(1, byteorder='little', signed=False)
 		return buffer
 
 
-class SecretLockTransaction:
+class SecretLockTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.SECRET_LOCK
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -3201,27 +7257,30 @@
 		'duration': 'pod:BlockDuration',
 		'hash_algorithm': 'enum:LockHashAlgorithm'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = SecretLockTransaction.TRANSACTION_VERSION
+		self._version = SecretLockTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = SecretLockTransaction.TRANSACTION_TYPE
+		self._type_ = SecretLockTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._recipient_address = UnresolvedAddress()
 		self._secret = Hash256()
 		self._mosaic = UnresolvedMosaic()
 		self._duration = BlockDuration()
 		self._hash_algorithm = LockHashAlgorithm.SHA3_256
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		self._mosaic.sort()
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -3331,15 +7390,15 @@
 		size += self.secret.size
 		size += self.mosaic.size
 		size += self.duration.size
 		size += self.hash_algorithm.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> SecretLockTransaction:
+	def deserialize(cls, payload: ByteString) -> SecretLockTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -3368,15 +7427,15 @@
 		mosaic = UnresolvedMosaic.deserialize(buffer)
 		buffer = buffer[mosaic.size:]
 		duration = BlockDuration.deserialize(buffer)
 		buffer = buffer[duration.size:]
 		hash_algorithm = LockHashAlgorithm.deserialize(buffer)
 		buffer = buffer[hash_algorithm.size:]
 
-		instance = SecretLockTransaction()
+		instance = SecretLockTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -3420,15 +7479,15 @@
 		result += f'mosaic: {self._mosaic.__str__()}, '
 		result += f'duration: {self._duration.__str__()}, '
 		result += f'hash_algorithm: {self._hash_algorithm.__str__()}, '
 		result += ')'
 		return result
 
 
-class EmbeddedSecretLockTransaction:
+class EmbeddedSecretLockTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.SECRET_LOCK
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'recipient_address': 'pod:UnresolvedAddress',
@@ -3436,25 +7495,28 @@
 		'mosaic': 'struct:UnresolvedMosaic',
 		'duration': 'pod:BlockDuration',
 		'hash_algorithm': 'enum:LockHashAlgorithm'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedSecretLockTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedSecretLockTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedSecretLockTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedSecretLockTransactionV1.TRANSACTION_TYPE
 		self._recipient_address = UnresolvedAddress()
 		self._secret = Hash256()
 		self._mosaic = UnresolvedMosaic()
 		self._duration = BlockDuration()
 		self._hash_algorithm = LockHashAlgorithm.SHA3_256
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		self._mosaic.sort()
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -3537,15 +7599,15 @@
 		size += self.secret.size
 		size += self.mosaic.size
 		size += self.duration.size
 		size += self.hash_algorithm.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedSecretLockTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedSecretLockTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -3568,15 +7630,15 @@
 		mosaic = UnresolvedMosaic.deserialize(buffer)
 		buffer = buffer[mosaic.size:]
 		duration = BlockDuration.deserialize(buffer)
 		buffer = buffer[duration.size:]
 		hash_algorithm = LockHashAlgorithm.deserialize(buffer)
 		buffer = buffer[hash_algorithm.size:]
 
-		instance = EmbeddedSecretLockTransaction()
+		instance = EmbeddedSecretLockTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._recipient_address = recipient_address
 		instance._secret = secret
 		instance._mosaic = mosaic
@@ -3611,15 +7673,15 @@
 		result += f'mosaic: {self._mosaic.__str__()}, '
 		result += f'duration: {self._duration.__str__()}, '
 		result += f'hash_algorithm: {self._hash_algorithm.__str__()}, '
 		result += ')'
 		return result
 
 
-class SecretProofTransaction:
+class SecretProofTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.SECRET_PROOF
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -3630,26 +7692,29 @@
 		'hash_algorithm': 'enum:LockHashAlgorithm',
 		'proof': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = SecretProofTransaction.TRANSACTION_VERSION
+		self._version = SecretProofTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = SecretProofTransaction.TRANSACTION_TYPE
+		self._type_ = SecretProofTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._recipient_address = UnresolvedAddress()
 		self._secret = Hash256()
 		self._hash_algorithm = LockHashAlgorithm.SHA3_256
 		self._proof = bytes()
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -3751,15 +7816,15 @@
 		size += self.secret.size
 		size += 2
 		size += self.hash_algorithm.size
 		size += len(self._proof)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> SecretProofTransaction:
+	def deserialize(cls, payload: ByteString) -> SecretProofTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -3788,15 +7853,15 @@
 		proof_size = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
 		hash_algorithm = LockHashAlgorithm.deserialize(buffer)
 		buffer = buffer[hash_algorithm.size:]
 		proof = ArrayHelpers.get_bytes(buffer, proof_size)
 		buffer = buffer[proof_size:]
 
-		instance = SecretProofTransaction()
+		instance = SecretProofTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -3838,39 +7903,42 @@
 		result += f'secret: {self._secret.__str__()}, '
 		result += f'hash_algorithm: {self._hash_algorithm.__str__()}, '
 		result += f'proof: {hexlify(self._proof).decode("utf8")}, '
 		result += ')'
 		return result
 
 
-class EmbeddedSecretProofTransaction:
+class EmbeddedSecretProofTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.SECRET_PROOF
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'recipient_address': 'pod:UnresolvedAddress',
 		'secret': 'pod:Hash256',
 		'hash_algorithm': 'enum:LockHashAlgorithm',
 		'proof': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedSecretProofTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedSecretProofTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedSecretProofTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedSecretProofTransactionV1.TRANSACTION_TYPE
 		self._recipient_address = UnresolvedAddress()
 		self._secret = Hash256()
 		self._hash_algorithm = LockHashAlgorithm.SHA3_256
 		self._proof = bytes()
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -3945,15 +8013,15 @@
 		size += self.secret.size
 		size += 2
 		size += self.hash_algorithm.size
 		size += len(self._proof)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedSecretProofTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedSecretProofTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -3976,15 +8044,15 @@
 		proof_size = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
 		hash_algorithm = LockHashAlgorithm.deserialize(buffer)
 		buffer = buffer[hash_algorithm.size:]
 		proof = ArrayHelpers.get_bytes(buffer, proof_size)
 		buffer = buffer[proof_size:]
 
-		instance = EmbeddedSecretProofTransaction()
+		instance = EmbeddedSecretProofTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._recipient_address = recipient_address
 		instance._secret = secret
 		instance._hash_algorithm = hash_algorithm
@@ -4017,15 +8085,15 @@
 		result += f'secret: {self._secret.__str__()}, '
 		result += f'hash_algorithm: {self._hash_algorithm.__str__()}, '
 		result += f'proof: {hexlify(self._proof).decode("utf8")}, '
 		result += ')'
 		return result
 
 
-class AccountMetadataTransaction:
+class AccountMetadataTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.ACCOUNT_METADATA
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -4034,26 +8102,29 @@
 		'target_address': 'pod:UnresolvedAddress',
 		'value': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = AccountMetadataTransaction.TRANSACTION_VERSION
+		self._version = AccountMetadataTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = AccountMetadataTransaction.TRANSACTION_TYPE
+		self._type_ = AccountMetadataTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._target_address = UnresolvedAddress()
 		self._scoped_metadata_key = 0
 		self._value_size_delta = 0
 		self._value = bytes()
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -4155,15 +8226,15 @@
 		size += 8
 		size += 2
 		size += 2
 		size += len(self._value)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> AccountMetadataTransaction:
+	def deserialize(cls, payload: ByteString) -> AccountMetadataTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -4192,15 +8263,15 @@
 		value_size_delta = int.from_bytes(buffer[:2], byteorder='little', signed=True)
 		buffer = buffer[2:]
 		value_size = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
 		value = ArrayHelpers.get_bytes(buffer, value_size)
 		buffer = buffer[value_size:]
 
-		instance = AccountMetadataTransaction()
+		instance = AccountMetadataTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -4242,37 +8313,40 @@
 		result += f'scoped_metadata_key: 0x{self._scoped_metadata_key:X}, '
 		result += f'value_size_delta: 0x{self._value_size_delta:X}, '
 		result += f'value: {hexlify(self._value).decode("utf8")}, '
 		result += ')'
 		return result
 
 
-class EmbeddedAccountMetadataTransaction:
+class EmbeddedAccountMetadataTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.ACCOUNT_METADATA
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'target_address': 'pod:UnresolvedAddress',
 		'value': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedAccountMetadataTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedAccountMetadataTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedAccountMetadataTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedAccountMetadataTransactionV1.TRANSACTION_TYPE
 		self._target_address = UnresolvedAddress()
 		self._scoped_metadata_key = 0
 		self._value_size_delta = 0
 		self._value = bytes()
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -4347,15 +8421,15 @@
 		size += 8
 		size += 2
 		size += 2
 		size += len(self._value)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedAccountMetadataTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedAccountMetadataTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -4378,15 +8452,15 @@
 		value_size_delta = int.from_bytes(buffer[:2], byteorder='little', signed=True)
 		buffer = buffer[2:]
 		value_size = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
 		value = ArrayHelpers.get_bytes(buffer, value_size)
 		buffer = buffer[value_size:]
 
-		instance = EmbeddedAccountMetadataTransaction()
+		instance = EmbeddedAccountMetadataTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._target_address = target_address
 		instance._scoped_metadata_key = scoped_metadata_key
 		instance._value_size_delta = value_size_delta
@@ -4419,15 +8493,15 @@
 		result += f'scoped_metadata_key: 0x{self._scoped_metadata_key:X}, '
 		result += f'value_size_delta: 0x{self._value_size_delta:X}, '
 		result += f'value: {hexlify(self._value).decode("utf8")}, '
 		result += ')'
 		return result
 
 
-class MosaicMetadataTransaction:
+class MosaicMetadataTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_METADATA
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -4437,27 +8511,30 @@
 		'target_mosaic_id': 'pod:UnresolvedMosaicId',
 		'value': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = MosaicMetadataTransaction.TRANSACTION_VERSION
+		self._version = MosaicMetadataTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = MosaicMetadataTransaction.TRANSACTION_TYPE
+		self._type_ = MosaicMetadataTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._target_address = UnresolvedAddress()
 		self._scoped_metadata_key = 0
 		self._target_mosaic_id = UnresolvedMosaicId()
 		self._value_size_delta = 0
 		self._value = bytes()
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -4568,15 +8645,15 @@
 		size += self.target_mosaic_id.size
 		size += 2
 		size += 2
 		size += len(self._value)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> MosaicMetadataTransaction:
+	def deserialize(cls, payload: ByteString) -> MosaicMetadataTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -4607,15 +8684,15 @@
 		value_size_delta = int.from_bytes(buffer[:2], byteorder='little', signed=True)
 		buffer = buffer[2:]
 		value_size = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
 		value = ArrayHelpers.get_bytes(buffer, value_size)
 		buffer = buffer[value_size:]
 
-		instance = MosaicMetadataTransaction()
+		instance = MosaicMetadataTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -4660,39 +8737,42 @@
 		result += f'target_mosaic_id: {self._target_mosaic_id.__str__()}, '
 		result += f'value_size_delta: 0x{self._value_size_delta:X}, '
 		result += f'value: {hexlify(self._value).decode("utf8")}, '
 		result += ')'
 		return result
 
 
-class EmbeddedMosaicMetadataTransaction:
+class EmbeddedMosaicMetadataTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_METADATA
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'target_address': 'pod:UnresolvedAddress',
 		'target_mosaic_id': 'pod:UnresolvedMosaicId',
 		'value': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedMosaicMetadataTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedMosaicMetadataTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedMosaicMetadataTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedMosaicMetadataTransactionV1.TRANSACTION_TYPE
 		self._target_address = UnresolvedAddress()
 		self._scoped_metadata_key = 0
 		self._target_mosaic_id = UnresolvedMosaicId()
 		self._value_size_delta = 0
 		self._value = bytes()
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -4776,15 +8856,15 @@
 		size += self.target_mosaic_id.size
 		size += 2
 		size += 2
 		size += len(self._value)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedMosaicMetadataTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedMosaicMetadataTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -4809,15 +8889,15 @@
 		value_size_delta = int.from_bytes(buffer[:2], byteorder='little', signed=True)
 		buffer = buffer[2:]
 		value_size = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
 		value = ArrayHelpers.get_bytes(buffer, value_size)
 		buffer = buffer[value_size:]
 
-		instance = EmbeddedMosaicMetadataTransaction()
+		instance = EmbeddedMosaicMetadataTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._target_address = target_address
 		instance._scoped_metadata_key = scoped_metadata_key
 		instance._target_mosaic_id = target_mosaic_id
@@ -4853,68 +8933,15 @@
 		result += f'target_mosaic_id: {self._target_mosaic_id.__str__()}, '
 		result += f'value_size_delta: 0x{self._value_size_delta:X}, '
 		result += f'value: {hexlify(self._value).decode("utf8")}, '
 		result += ')'
 		return result
 
 
-class NamespaceId(BaseValue):
-	SIZE = 8
-
-	def __init__(self, namespace_id: int = 0):
-		super().__init__(self.SIZE, namespace_id, NamespaceId)
-
-	@classmethod
-	def deserialize(cls, payload: ByteString) -> NamespaceId:
-		buffer = memoryview(payload)
-		return NamespaceId(int.from_bytes(buffer[:8], byteorder='little', signed=False))
-
-	def serialize(self) -> bytes:
-		return self.value.to_bytes(8, byteorder='little', signed=False)
-
-
-class NamespaceRegistrationType(Enum):
-	ROOT = 0
-	CHILD = 1
-
-	@property
-	def size(self) -> int:
-		return 1
-
-	@classmethod
-	def deserialize(cls, payload: ByteString) -> NamespaceRegistrationType:
-		buffer = memoryview(payload)
-		return NamespaceRegistrationType(int.from_bytes(buffer[:1], byteorder='little', signed=False))
-
-	def serialize(self) -> bytes:
-		buffer = bytes()
-		buffer += self.value.to_bytes(1, byteorder='little', signed=False)
-		return buffer
-
-
-class AliasAction(Enum):
-	UNLINK = 0
-	LINK = 1
-
-	@property
-	def size(self) -> int:
-		return 1
-
-	@classmethod
-	def deserialize(cls, payload: ByteString) -> AliasAction:
-		buffer = memoryview(payload)
-		return AliasAction(int.from_bytes(buffer[:1], byteorder='little', signed=False))
-
-	def serialize(self) -> bytes:
-		buffer = bytes()
-		buffer += self.value.to_bytes(1, byteorder='little', signed=False)
-		return buffer
-
-
-class NamespaceMetadataTransaction:
+class NamespaceMetadataTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.NAMESPACE_METADATA
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -4924,27 +8951,30 @@
 		'target_namespace_id': 'pod:NamespaceId',
 		'value': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = NamespaceMetadataTransaction.TRANSACTION_VERSION
+		self._version = NamespaceMetadataTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = NamespaceMetadataTransaction.TRANSACTION_TYPE
+		self._type_ = NamespaceMetadataTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._target_address = UnresolvedAddress()
 		self._scoped_metadata_key = 0
 		self._target_namespace_id = NamespaceId()
 		self._value_size_delta = 0
 		self._value = bytes()
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -5055,15 +9085,15 @@
 		size += self.target_namespace_id.size
 		size += 2
 		size += 2
 		size += len(self._value)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> NamespaceMetadataTransaction:
+	def deserialize(cls, payload: ByteString) -> NamespaceMetadataTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -5094,15 +9124,15 @@
 		value_size_delta = int.from_bytes(buffer[:2], byteorder='little', signed=True)
 		buffer = buffer[2:]
 		value_size = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
 		value = ArrayHelpers.get_bytes(buffer, value_size)
 		buffer = buffer[value_size:]
 
-		instance = NamespaceMetadataTransaction()
+		instance = NamespaceMetadataTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -5147,39 +9177,42 @@
 		result += f'target_namespace_id: {self._target_namespace_id.__str__()}, '
 		result += f'value_size_delta: 0x{self._value_size_delta:X}, '
 		result += f'value: {hexlify(self._value).decode("utf8")}, '
 		result += ')'
 		return result
 
 
-class EmbeddedNamespaceMetadataTransaction:
+class EmbeddedNamespaceMetadataTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.NAMESPACE_METADATA
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'target_address': 'pod:UnresolvedAddress',
 		'target_namespace_id': 'pod:NamespaceId',
 		'value': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedNamespaceMetadataTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedNamespaceMetadataTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedNamespaceMetadataTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedNamespaceMetadataTransactionV1.TRANSACTION_TYPE
 		self._target_address = UnresolvedAddress()
 		self._scoped_metadata_key = 0
 		self._target_namespace_id = NamespaceId()
 		self._value_size_delta = 0
 		self._value = bytes()
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -5263,15 +9296,15 @@
 		size += self.target_namespace_id.size
 		size += 2
 		size += 2
 		size += len(self._value)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedNamespaceMetadataTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedNamespaceMetadataTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -5296,15 +9329,15 @@
 		value_size_delta = int.from_bytes(buffer[:2], byteorder='little', signed=True)
 		buffer = buffer[2:]
 		value_size = int.from_bytes(buffer[:2], byteorder='little', signed=False)
 		buffer = buffer[2:]
 		value = ArrayHelpers.get_bytes(buffer, value_size)
 		buffer = buffer[value_size:]
 
-		instance = EmbeddedNamespaceMetadataTransaction()
+		instance = EmbeddedNamespaceMetadataTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._target_address = target_address
 		instance._scoped_metadata_key = scoped_metadata_key
 		instance._target_namespace_id = target_namespace_id
@@ -5396,15 +9429,15 @@
 
 	def serialize(self) -> bytes:
 		buffer = bytes()
 		buffer += self.value.to_bytes(1, byteorder='little', signed=False)
 		return buffer
 
 
-class MosaicDefinitionTransaction:
+class MosaicDefinitionTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_DEFINITION
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -5415,27 +9448,30 @@
 		'nonce': 'pod:MosaicNonce',
 		'flags': 'enum:MosaicFlags'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = MosaicDefinitionTransaction.TRANSACTION_VERSION
+		self._version = MosaicDefinitionTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = MosaicDefinitionTransaction.TRANSACTION_TYPE
+		self._type_ = MosaicDefinitionTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._id = MosaicId()
 		self._duration = BlockDuration()
 		self._nonce = MosaicNonce()
 		self._flags = MosaicFlags.NONE
 		self._divisibility = 0
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -5545,15 +9581,15 @@
 		size += self.duration.size
 		size += self.nonce.size
 		size += self.flags.size
 		size += 1
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> MosaicDefinitionTransaction:
+	def deserialize(cls, payload: ByteString) -> MosaicDefinitionTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -5582,15 +9618,15 @@
 		nonce = MosaicNonce.deserialize(buffer)
 		buffer = buffer[nonce.size:]
 		flags = MosaicFlags.deserialize(buffer)
 		buffer = buffer[flags.size:]
 		divisibility = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 
-		instance = MosaicDefinitionTransaction()
+		instance = MosaicDefinitionTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -5634,40 +9670,43 @@
 		result += f'nonce: {self._nonce.__str__()}, '
 		result += f'flags: {self._flags.__str__()}, '
 		result += f'divisibility: 0x{self._divisibility:X}, '
 		result += ')'
 		return result
 
 
-class EmbeddedMosaicDefinitionTransaction:
+class EmbeddedMosaicDefinitionTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_DEFINITION
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'id': 'pod:MosaicId',
 		'duration': 'pod:BlockDuration',
 		'nonce': 'pod:MosaicNonce',
 		'flags': 'enum:MosaicFlags'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedMosaicDefinitionTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedMosaicDefinitionTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedMosaicDefinitionTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedMosaicDefinitionTransactionV1.TRANSACTION_TYPE
 		self._id = MosaicId()
 		self._duration = BlockDuration()
 		self._nonce = MosaicNonce()
 		self._flags = MosaicFlags.NONE
 		self._divisibility = 0
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -5750,15 +9789,15 @@
 		size += self.duration.size
 		size += self.nonce.size
 		size += self.flags.size
 		size += 1
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedMosaicDefinitionTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedMosaicDefinitionTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -5781,15 +9820,15 @@
 		nonce = MosaicNonce.deserialize(buffer)
 		buffer = buffer[nonce.size:]
 		flags = MosaicFlags.deserialize(buffer)
 		buffer = buffer[flags.size:]
 		divisibility = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 
-		instance = EmbeddedMosaicDefinitionTransaction()
+		instance = EmbeddedMosaicDefinitionTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._id = id
 		instance._duration = duration
 		instance._nonce = nonce
@@ -5824,15 +9863,15 @@
 		result += f'nonce: {self._nonce.__str__()}, '
 		result += f'flags: {self._flags.__str__()}, '
 		result += f'divisibility: 0x{self._divisibility:X}, '
 		result += ')'
 		return result
 
 
-class MosaicSupplyChangeTransaction:
+class MosaicSupplyChangeTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_SUPPLY_CHANGE
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -5842,25 +9881,28 @@
 		'delta': 'pod:Amount',
 		'action': 'enum:MosaicSupplyChangeAction'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = MosaicSupplyChangeTransaction.TRANSACTION_VERSION
+		self._version = MosaicSupplyChangeTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = MosaicSupplyChangeTransaction.TRANSACTION_TYPE
+		self._type_ = MosaicSupplyChangeTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._mosaic_id = UnresolvedMosaicId()
 		self._delta = Amount()
 		self._action = MosaicSupplyChangeAction.DECREASE
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -5952,15 +9994,15 @@
 		size += self.deadline.size
 		size += self.mosaic_id.size
 		size += self.delta.size
 		size += self.action.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> MosaicSupplyChangeTransaction:
+	def deserialize(cls, payload: ByteString) -> MosaicSupplyChangeTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -5985,15 +10027,15 @@
 		mosaic_id = UnresolvedMosaicId.deserialize(buffer)
 		buffer = buffer[mosaic_id.size:]
 		delta = Amount.deserialize(buffer)
 		buffer = buffer[delta.size:]
 		action = MosaicSupplyChangeAction.deserialize(buffer)
 		buffer = buffer[action.size:]
 
-		instance = MosaicSupplyChangeTransaction()
+		instance = MosaicSupplyChangeTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -6031,37 +10073,40 @@
 		result += f'mosaic_id: {self._mosaic_id.__str__()}, '
 		result += f'delta: {self._delta.__str__()}, '
 		result += f'action: {self._action.__str__()}, '
 		result += ')'
 		return result
 
 
-class EmbeddedMosaicSupplyChangeTransaction:
+class EmbeddedMosaicSupplyChangeTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_SUPPLY_CHANGE
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'mosaic_id': 'pod:UnresolvedMosaicId',
 		'delta': 'pod:Amount',
 		'action': 'enum:MosaicSupplyChangeAction'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedMosaicSupplyChangeTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedMosaicSupplyChangeTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedMosaicSupplyChangeTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedMosaicSupplyChangeTransactionV1.TRANSACTION_TYPE
 		self._mosaic_id = UnresolvedMosaicId()
 		self._delta = Amount()
 		self._action = MosaicSupplyChangeAction.DECREASE
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -6126,15 +10171,15 @@
 		size += self.type_.size
 		size += self.mosaic_id.size
 		size += self.delta.size
 		size += self.action.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedMosaicSupplyChangeTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedMosaicSupplyChangeTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -6153,15 +10198,15 @@
 		mosaic_id = UnresolvedMosaicId.deserialize(buffer)
 		buffer = buffer[mosaic_id.size:]
 		delta = Amount.deserialize(buffer)
 		buffer = buffer[delta.size:]
 		action = MosaicSupplyChangeAction.deserialize(buffer)
 		buffer = buffer[action.size:]
 
-		instance = EmbeddedMosaicSupplyChangeTransaction()
+		instance = EmbeddedMosaicSupplyChangeTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._mosaic_id = mosaic_id
 		instance._delta = delta
 		instance._action = action
@@ -6190,15 +10235,15 @@
 		result += f'mosaic_id: {self._mosaic_id.__str__()}, '
 		result += f'delta: {self._delta.__str__()}, '
 		result += f'action: {self._action.__str__()}, '
 		result += ')'
 		return result
 
 
-class MosaicSupplyRevocationTransaction:
+class MosaicSupplyRevocationTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_SUPPLY_REVOCATION
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -6207,24 +10252,27 @@
 		'source_address': 'pod:UnresolvedAddress',
 		'mosaic': 'struct:UnresolvedMosaic'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = MosaicSupplyRevocationTransaction.TRANSACTION_VERSION
+		self._version = MosaicSupplyRevocationTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = MosaicSupplyRevocationTransaction.TRANSACTION_TYPE
+		self._type_ = MosaicSupplyRevocationTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._source_address = UnresolvedAddress()
 		self._mosaic = UnresolvedMosaic()
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		self._mosaic.sort()
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -6307,15 +10355,15 @@
 		size += self.fee.size
 		size += self.deadline.size
 		size += self.source_address.size
 		size += self.mosaic.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> MosaicSupplyRevocationTransaction:
+	def deserialize(cls, payload: ByteString) -> MosaicSupplyRevocationTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -6338,15 +10386,15 @@
 		deadline = Timestamp.deserialize(buffer)
 		buffer = buffer[deadline.size:]
 		source_address = UnresolvedAddress.deserialize(buffer)
 		buffer = buffer[source_address.size:]
 		mosaic = UnresolvedMosaic.deserialize(buffer)
 		buffer = buffer[mosaic.size:]
 
-		instance = MosaicSupplyRevocationTransaction()
+		instance = MosaicSupplyRevocationTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -6381,35 +10429,38 @@
 		result += f'deadline: {self._deadline.__str__()}, '
 		result += f'source_address: {self._source_address.__str__()}, '
 		result += f'mosaic: {self._mosaic.__str__()}, '
 		result += ')'
 		return result
 
 
-class EmbeddedMosaicSupplyRevocationTransaction:
+class EmbeddedMosaicSupplyRevocationTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_SUPPLY_REVOCATION
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'source_address': 'pod:UnresolvedAddress',
 		'mosaic': 'struct:UnresolvedMosaic'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedMosaicSupplyRevocationTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedMosaicSupplyRevocationTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedMosaicSupplyRevocationTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedMosaicSupplyRevocationTransactionV1.TRANSACTION_TYPE
 		self._source_address = UnresolvedAddress()
 		self._mosaic = UnresolvedMosaic()
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		self._mosaic.sort()
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -6465,15 +10516,15 @@
 		size += self.network.size
 		size += self.type_.size
 		size += self.source_address.size
 		size += self.mosaic.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedMosaicSupplyRevocationTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedMosaicSupplyRevocationTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -6490,15 +10541,15 @@
 		type_ = TransactionType.deserialize(buffer)
 		buffer = buffer[type_.size:]
 		source_address = UnresolvedAddress.deserialize(buffer)
 		buffer = buffer[source_address.size:]
 		mosaic = UnresolvedMosaic.deserialize(buffer)
 		buffer = buffer[mosaic.size:]
 
-		instance = EmbeddedMosaicSupplyRevocationTransaction()
+		instance = EmbeddedMosaicSupplyRevocationTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._source_address = source_address
 		instance._mosaic = mosaic
 		return instance
@@ -6524,15 +10575,15 @@
 		result += f'type_: {self._type_.__str__()}, '
 		result += f'source_address: {self._source_address.__str__()}, '
 		result += f'mosaic: {self._mosaic.__str__()}, '
 		result += ')'
 		return result
 
 
-class MultisigAccountModificationTransaction:
+class MultisigAccountModificationTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MULTISIG_ACCOUNT_MODIFICATION
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -6541,27 +10592,30 @@
 		'address_additions': 'array[UnresolvedAddress]',
 		'address_deletions': 'array[UnresolvedAddress]'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = MultisigAccountModificationTransaction.TRANSACTION_VERSION
+		self._version = MultisigAccountModificationTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = MultisigAccountModificationTransaction.TRANSACTION_TYPE
+		self._type_ = MultisigAccountModificationTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._min_removal_delta = 0
 		self._min_approval_delta = 0
 		self._address_additions = []
 		self._address_deletions = []
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._multisig_account_modification_transaction_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -6665,15 +10719,15 @@
 		size += 1
 		size += 4
 		size += ArrayHelpers.size(self.address_additions)
 		size += ArrayHelpers.size(self.address_deletions)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> MultisigAccountModificationTransaction:
+	def deserialize(cls, payload: ByteString) -> MultisigAccountModificationTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -6707,15 +10761,15 @@
 		buffer = buffer[4:]
 		assert multisig_account_modification_transaction_body_reserved_1 == 0, f'Invalid value of reserved field ({multisig_account_modification_transaction_body_reserved_1})'
 		address_additions = ArrayHelpers.read_array_count(buffer, UnresolvedAddress, address_additions_count)
 		buffer = buffer[ArrayHelpers.size(address_additions):]
 		address_deletions = ArrayHelpers.read_array_count(buffer, UnresolvedAddress, address_deletions_count)
 		buffer = buffer[ArrayHelpers.size(address_deletions):]
 
-		instance = MultisigAccountModificationTransaction()
+		instance = MultisigAccountModificationTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -6759,38 +10813,41 @@
 		result += f'min_approval_delta: 0x{self._min_approval_delta:X}, '
 		result += f'address_additions: {list(map(str, self._address_additions))}, '
 		result += f'address_deletions: {list(map(str, self._address_deletions))}, '
 		result += ')'
 		return result
 
 
-class EmbeddedMultisigAccountModificationTransaction:
+class EmbeddedMultisigAccountModificationTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MULTISIG_ACCOUNT_MODIFICATION
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'address_additions': 'array[UnresolvedAddress]',
 		'address_deletions': 'array[UnresolvedAddress]'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedMultisigAccountModificationTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedMultisigAccountModificationTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedMultisigAccountModificationTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedMultisigAccountModificationTransactionV1.TRANSACTION_TYPE
 		self._min_removal_delta = 0
 		self._min_approval_delta = 0
 		self._address_additions = []
 		self._address_deletions = []
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._multisig_account_modification_transaction_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -6867,15 +10924,15 @@
 		size += 1
 		size += 4
 		size += ArrayHelpers.size(self.address_additions)
 		size += ArrayHelpers.size(self.address_deletions)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedMultisigAccountModificationTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedMultisigAccountModificationTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -6903,15 +10960,15 @@
 		buffer = buffer[4:]
 		assert multisig_account_modification_transaction_body_reserved_1 == 0, f'Invalid value of reserved field ({multisig_account_modification_transaction_body_reserved_1})'
 		address_additions = ArrayHelpers.read_array_count(buffer, UnresolvedAddress, address_additions_count)
 		buffer = buffer[ArrayHelpers.size(address_additions):]
 		address_deletions = ArrayHelpers.read_array_count(buffer, UnresolvedAddress, address_deletions_count)
 		buffer = buffer[ArrayHelpers.size(address_deletions):]
 
-		instance = EmbeddedMultisigAccountModificationTransaction()
+		instance = EmbeddedMultisigAccountModificationTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._min_removal_delta = min_removal_delta
 		instance._min_approval_delta = min_approval_delta
 		instance._address_additions = address_additions
@@ -6946,15 +11003,15 @@
 		result += f'min_approval_delta: 0x{self._min_approval_delta:X}, '
 		result += f'address_additions: {list(map(str, self._address_additions))}, '
 		result += f'address_deletions: {list(map(str, self._address_deletions))}, '
 		result += ')'
 		return result
 
 
-class AddressAliasTransaction:
+class AddressAliasTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.ADDRESS_ALIAS
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -6964,25 +11021,28 @@
 		'address': 'pod:Address',
 		'alias_action': 'enum:AliasAction'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = AddressAliasTransaction.TRANSACTION_VERSION
+		self._version = AddressAliasTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = AddressAliasTransaction.TRANSACTION_TYPE
+		self._type_ = AddressAliasTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._namespace_id = NamespaceId()
 		self._address = Address()
 		self._alias_action = AliasAction.UNLINK
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -7074,15 +11134,15 @@
 		size += self.deadline.size
 		size += self.namespace_id.size
 		size += self.address.size
 		size += self.alias_action.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> AddressAliasTransaction:
+	def deserialize(cls, payload: ByteString) -> AddressAliasTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -7107,15 +11167,15 @@
 		namespace_id = NamespaceId.deserialize(buffer)
 		buffer = buffer[namespace_id.size:]
 		address = Address.deserialize(buffer)
 		buffer = buffer[address.size:]
 		alias_action = AliasAction.deserialize(buffer)
 		buffer = buffer[alias_action.size:]
 
-		instance = AddressAliasTransaction()
+		instance = AddressAliasTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -7153,37 +11213,40 @@
 		result += f'namespace_id: {self._namespace_id.__str__()}, '
 		result += f'address: {self._address.__str__()}, '
 		result += f'alias_action: {self._alias_action.__str__()}, '
 		result += ')'
 		return result
 
 
-class EmbeddedAddressAliasTransaction:
+class EmbeddedAddressAliasTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.ADDRESS_ALIAS
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'namespace_id': 'pod:NamespaceId',
 		'address': 'pod:Address',
 		'alias_action': 'enum:AliasAction'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedAddressAliasTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedAddressAliasTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedAddressAliasTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedAddressAliasTransactionV1.TRANSACTION_TYPE
 		self._namespace_id = NamespaceId()
 		self._address = Address()
 		self._alias_action = AliasAction.UNLINK
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -7248,15 +11311,15 @@
 		size += self.type_.size
 		size += self.namespace_id.size
 		size += self.address.size
 		size += self.alias_action.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedAddressAliasTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedAddressAliasTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -7275,15 +11338,15 @@
 		namespace_id = NamespaceId.deserialize(buffer)
 		buffer = buffer[namespace_id.size:]
 		address = Address.deserialize(buffer)
 		buffer = buffer[address.size:]
 		alias_action = AliasAction.deserialize(buffer)
 		buffer = buffer[alias_action.size:]
 
-		instance = EmbeddedAddressAliasTransaction()
+		instance = EmbeddedAddressAliasTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._namespace_id = namespace_id
 		instance._address = address
 		instance._alias_action = alias_action
@@ -7312,15 +11375,15 @@
 		result += f'namespace_id: {self._namespace_id.__str__()}, '
 		result += f'address: {self._address.__str__()}, '
 		result += f'alias_action: {self._alias_action.__str__()}, '
 		result += ')'
 		return result
 
 
-class MosaicAliasTransaction:
+class MosaicAliasTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_ALIAS
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -7330,25 +11393,28 @@
 		'mosaic_id': 'pod:MosaicId',
 		'alias_action': 'enum:AliasAction'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = MosaicAliasTransaction.TRANSACTION_VERSION
+		self._version = MosaicAliasTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = MosaicAliasTransaction.TRANSACTION_TYPE
+		self._type_ = MosaicAliasTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._namespace_id = NamespaceId()
 		self._mosaic_id = MosaicId()
 		self._alias_action = AliasAction.UNLINK
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -7440,15 +11506,15 @@
 		size += self.deadline.size
 		size += self.namespace_id.size
 		size += self.mosaic_id.size
 		size += self.alias_action.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> MosaicAliasTransaction:
+	def deserialize(cls, payload: ByteString) -> MosaicAliasTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -7473,15 +11539,15 @@
 		namespace_id = NamespaceId.deserialize(buffer)
 		buffer = buffer[namespace_id.size:]
 		mosaic_id = MosaicId.deserialize(buffer)
 		buffer = buffer[mosaic_id.size:]
 		alias_action = AliasAction.deserialize(buffer)
 		buffer = buffer[alias_action.size:]
 
-		instance = MosaicAliasTransaction()
+		instance = MosaicAliasTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -7519,37 +11585,40 @@
 		result += f'namespace_id: {self._namespace_id.__str__()}, '
 		result += f'mosaic_id: {self._mosaic_id.__str__()}, '
 		result += f'alias_action: {self._alias_action.__str__()}, '
 		result += ')'
 		return result
 
 
-class EmbeddedMosaicAliasTransaction:
+class EmbeddedMosaicAliasTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_ALIAS
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'namespace_id': 'pod:NamespaceId',
 		'mosaic_id': 'pod:MosaicId',
 		'alias_action': 'enum:AliasAction'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedMosaicAliasTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedMosaicAliasTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedMosaicAliasTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedMosaicAliasTransactionV1.TRANSACTION_TYPE
 		self._namespace_id = NamespaceId()
 		self._mosaic_id = MosaicId()
 		self._alias_action = AliasAction.UNLINK
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -7614,15 +11683,15 @@
 		size += self.type_.size
 		size += self.namespace_id.size
 		size += self.mosaic_id.size
 		size += self.alias_action.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedMosaicAliasTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedMosaicAliasTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -7641,15 +11710,15 @@
 		namespace_id = NamespaceId.deserialize(buffer)
 		buffer = buffer[namespace_id.size:]
 		mosaic_id = MosaicId.deserialize(buffer)
 		buffer = buffer[mosaic_id.size:]
 		alias_action = AliasAction.deserialize(buffer)
 		buffer = buffer[alias_action.size:]
 
-		instance = EmbeddedMosaicAliasTransaction()
+		instance = EmbeddedMosaicAliasTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._namespace_id = namespace_id
 		instance._mosaic_id = mosaic_id
 		instance._alias_action = alias_action
@@ -7678,15 +11747,15 @@
 		result += f'namespace_id: {self._namespace_id.__str__()}, '
 		result += f'mosaic_id: {self._mosaic_id.__str__()}, '
 		result += f'alias_action: {self._alias_action.__str__()}, '
 		result += ')'
 		return result
 
 
-class NamespaceRegistrationTransaction:
+class NamespaceRegistrationTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.NAMESPACE_REGISTRATION
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -7698,27 +11767,30 @@
 		'registration_type': 'enum:NamespaceRegistrationType',
 		'name': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = NamespaceRegistrationTransaction.TRANSACTION_VERSION
+		self._version = NamespaceRegistrationTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = NamespaceRegistrationTransaction.TRANSACTION_TYPE
+		self._type_ = NamespaceRegistrationTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._duration = BlockDuration()
-		self._parent_id = NamespaceId()
+		self._parent_id = None
 		self._id = NamespaceId()
 		self._registration_type = NamespaceRegistrationType.ROOT
 		self._name = bytes()
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -7831,15 +11903,15 @@
 		size += self.id.size
 		size += self.registration_type.size
 		size += 1
 		size += len(self._name)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> NamespaceRegistrationTransaction:
+	def deserialize(cls, payload: ByteString) -> NamespaceRegistrationTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -7879,15 +11951,15 @@
 			parent_id = NamespaceId.deserialize(registration_type_condition)
 			registration_type_condition = registration_type_condition[parent_id.size:]
 		name_size = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		name = ArrayHelpers.get_bytes(buffer, name_size)
 		buffer = buffer[name_size:]
 
-		instance = NamespaceRegistrationTransaction()
+		instance = NamespaceRegistrationTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -7936,15 +12008,15 @@
 		result += f'id: {self._id.__str__()}, '
 		result += f'registration_type: {self._registration_type.__str__()}, '
 		result += f'name: {hexlify(self._name).decode("utf8")}, '
 		result += ')'
 		return result
 
 
-class EmbeddedNamespaceRegistrationTransaction:
+class EmbeddedNamespaceRegistrationTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.NAMESPACE_REGISTRATION
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'duration': 'pod:BlockDuration',
@@ -7952,25 +12024,28 @@
 		'id': 'pod:NamespaceId',
 		'registration_type': 'enum:NamespaceRegistrationType',
 		'name': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedNamespaceRegistrationTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedNamespaceRegistrationTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedNamespaceRegistrationTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedNamespaceRegistrationTransactionV1.TRANSACTION_TYPE
 		self._duration = BlockDuration()
-		self._parent_id = NamespaceId()
+		self._parent_id = None
 		self._id = NamespaceId()
 		self._registration_type = NamespaceRegistrationType.ROOT
 		self._name = bytes()
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -8056,15 +12131,15 @@
 		size += self.id.size
 		size += self.registration_type.size
 		size += 1
 		size += len(self._name)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedNamespaceRegistrationTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedNamespaceRegistrationTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -8098,15 +12173,15 @@
 			parent_id = NamespaceId.deserialize(registration_type_condition)
 			registration_type_condition = registration_type_condition[parent_id.size:]
 		name_size = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		name = ArrayHelpers.get_bytes(buffer, name_size)
 		buffer = buffer[name_size:]
 
-		instance = EmbeddedNamespaceRegistrationTransaction()
+		instance = EmbeddedNamespaceRegistrationTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._duration = duration
 		instance._parent_id = parent_id
 		instance._id = id
@@ -8168,15 +12243,15 @@
 
 	def serialize(self) -> bytes:
 		buffer = bytes()
 		buffer += self.value.to_bytes(2, byteorder='little', signed=False)
 		return buffer
 
 
-class AccountAddressRestrictionTransaction:
+class AccountAddressRestrictionTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.ACCOUNT_ADDRESS_RESTRICTION
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -8186,26 +12261,29 @@
 		'restriction_additions': 'array[UnresolvedAddress]',
 		'restriction_deletions': 'array[UnresolvedAddress]'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = AccountAddressRestrictionTransaction.TRANSACTION_VERSION
+		self._version = AccountAddressRestrictionTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = AccountAddressRestrictionTransaction.TRANSACTION_TYPE
+		self._type_ = AccountAddressRestrictionTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._restriction_flags = AccountRestrictionFlags.ADDRESS
 		self._restriction_additions = []
 		self._restriction_deletions = []
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._account_restriction_transaction_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -8300,15 +12378,15 @@
 		size += 1
 		size += 4
 		size += ArrayHelpers.size(self.restriction_additions)
 		size += ArrayHelpers.size(self.restriction_deletions)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> AccountAddressRestrictionTransaction:
+	def deserialize(cls, payload: ByteString) -> AccountAddressRestrictionTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -8340,15 +12418,15 @@
 		buffer = buffer[4:]
 		assert account_restriction_transaction_body_reserved_1 == 0, f'Invalid value of reserved field ({account_restriction_transaction_body_reserved_1})'
 		restriction_additions = ArrayHelpers.read_array_count(buffer, UnresolvedAddress, restriction_additions_count)
 		buffer = buffer[ArrayHelpers.size(restriction_additions):]
 		restriction_deletions = ArrayHelpers.read_array_count(buffer, UnresolvedAddress, restriction_deletions_count)
 		buffer = buffer[ArrayHelpers.size(restriction_deletions):]
 
-		instance = AccountAddressRestrictionTransaction()
+		instance = AccountAddressRestrictionTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -8389,38 +12467,41 @@
 		result += f'restriction_flags: {self._restriction_flags.__str__()}, '
 		result += f'restriction_additions: {list(map(str, self._restriction_additions))}, '
 		result += f'restriction_deletions: {list(map(str, self._restriction_deletions))}, '
 		result += ')'
 		return result
 
 
-class EmbeddedAccountAddressRestrictionTransaction:
+class EmbeddedAccountAddressRestrictionTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.ACCOUNT_ADDRESS_RESTRICTION
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'restriction_flags': 'enum:AccountRestrictionFlags',
 		'restriction_additions': 'array[UnresolvedAddress]',
 		'restriction_deletions': 'array[UnresolvedAddress]'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedAccountAddressRestrictionTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedAccountAddressRestrictionTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedAccountAddressRestrictionTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedAccountAddressRestrictionTransactionV1.TRANSACTION_TYPE
 		self._restriction_flags = AccountRestrictionFlags.ADDRESS
 		self._restriction_additions = []
 		self._restriction_deletions = []
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._account_restriction_transaction_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -8488,15 +12569,15 @@
 		size += 1
 		size += 4
 		size += ArrayHelpers.size(self.restriction_additions)
 		size += ArrayHelpers.size(self.restriction_deletions)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedAccountAddressRestrictionTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedAccountAddressRestrictionTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -8522,15 +12603,15 @@
 		buffer = buffer[4:]
 		assert account_restriction_transaction_body_reserved_1 == 0, f'Invalid value of reserved field ({account_restriction_transaction_body_reserved_1})'
 		restriction_additions = ArrayHelpers.read_array_count(buffer, UnresolvedAddress, restriction_additions_count)
 		buffer = buffer[ArrayHelpers.size(restriction_additions):]
 		restriction_deletions = ArrayHelpers.read_array_count(buffer, UnresolvedAddress, restriction_deletions_count)
 		buffer = buffer[ArrayHelpers.size(restriction_deletions):]
 
-		instance = EmbeddedAccountAddressRestrictionTransaction()
+		instance = EmbeddedAccountAddressRestrictionTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._restriction_flags = restriction_flags
 		instance._restriction_additions = restriction_additions
 		instance._restriction_deletions = restriction_deletions
@@ -8562,15 +12643,15 @@
 		result += f'restriction_flags: {self._restriction_flags.__str__()}, '
 		result += f'restriction_additions: {list(map(str, self._restriction_additions))}, '
 		result += f'restriction_deletions: {list(map(str, self._restriction_deletions))}, '
 		result += ')'
 		return result
 
 
-class AccountMosaicRestrictionTransaction:
+class AccountMosaicRestrictionTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.ACCOUNT_MOSAIC_RESTRICTION
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -8580,26 +12661,29 @@
 		'restriction_additions': 'array[UnresolvedMosaicId]',
 		'restriction_deletions': 'array[UnresolvedMosaicId]'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = AccountMosaicRestrictionTransaction.TRANSACTION_VERSION
+		self._version = AccountMosaicRestrictionTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = AccountMosaicRestrictionTransaction.TRANSACTION_TYPE
+		self._type_ = AccountMosaicRestrictionTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._restriction_flags = AccountRestrictionFlags.ADDRESS
 		self._restriction_additions = []
 		self._restriction_deletions = []
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._account_restriction_transaction_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -8694,15 +12778,15 @@
 		size += 1
 		size += 4
 		size += ArrayHelpers.size(self.restriction_additions)
 		size += ArrayHelpers.size(self.restriction_deletions)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> AccountMosaicRestrictionTransaction:
+	def deserialize(cls, payload: ByteString) -> AccountMosaicRestrictionTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -8734,15 +12818,15 @@
 		buffer = buffer[4:]
 		assert account_restriction_transaction_body_reserved_1 == 0, f'Invalid value of reserved field ({account_restriction_transaction_body_reserved_1})'
 		restriction_additions = ArrayHelpers.read_array_count(buffer, UnresolvedMosaicId, restriction_additions_count)
 		buffer = buffer[ArrayHelpers.size(restriction_additions):]
 		restriction_deletions = ArrayHelpers.read_array_count(buffer, UnresolvedMosaicId, restriction_deletions_count)
 		buffer = buffer[ArrayHelpers.size(restriction_deletions):]
 
-		instance = AccountMosaicRestrictionTransaction()
+		instance = AccountMosaicRestrictionTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -8783,38 +12867,41 @@
 		result += f'restriction_flags: {self._restriction_flags.__str__()}, '
 		result += f'restriction_additions: {list(map(str, self._restriction_additions))}, '
 		result += f'restriction_deletions: {list(map(str, self._restriction_deletions))}, '
 		result += ')'
 		return result
 
 
-class EmbeddedAccountMosaicRestrictionTransaction:
+class EmbeddedAccountMosaicRestrictionTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.ACCOUNT_MOSAIC_RESTRICTION
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'restriction_flags': 'enum:AccountRestrictionFlags',
 		'restriction_additions': 'array[UnresolvedMosaicId]',
 		'restriction_deletions': 'array[UnresolvedMosaicId]'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedAccountMosaicRestrictionTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedAccountMosaicRestrictionTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedAccountMosaicRestrictionTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedAccountMosaicRestrictionTransactionV1.TRANSACTION_TYPE
 		self._restriction_flags = AccountRestrictionFlags.ADDRESS
 		self._restriction_additions = []
 		self._restriction_deletions = []
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._account_restriction_transaction_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -8882,15 +12969,15 @@
 		size += 1
 		size += 4
 		size += ArrayHelpers.size(self.restriction_additions)
 		size += ArrayHelpers.size(self.restriction_deletions)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedAccountMosaicRestrictionTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedAccountMosaicRestrictionTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -8916,15 +13003,15 @@
 		buffer = buffer[4:]
 		assert account_restriction_transaction_body_reserved_1 == 0, f'Invalid value of reserved field ({account_restriction_transaction_body_reserved_1})'
 		restriction_additions = ArrayHelpers.read_array_count(buffer, UnresolvedMosaicId, restriction_additions_count)
 		buffer = buffer[ArrayHelpers.size(restriction_additions):]
 		restriction_deletions = ArrayHelpers.read_array_count(buffer, UnresolvedMosaicId, restriction_deletions_count)
 		buffer = buffer[ArrayHelpers.size(restriction_deletions):]
 
-		instance = EmbeddedAccountMosaicRestrictionTransaction()
+		instance = EmbeddedAccountMosaicRestrictionTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._restriction_flags = restriction_flags
 		instance._restriction_additions = restriction_additions
 		instance._restriction_deletions = restriction_deletions
@@ -8956,15 +13043,15 @@
 		result += f'restriction_flags: {self._restriction_flags.__str__()}, '
 		result += f'restriction_additions: {list(map(str, self._restriction_additions))}, '
 		result += f'restriction_deletions: {list(map(str, self._restriction_deletions))}, '
 		result += ')'
 		return result
 
 
-class AccountOperationRestrictionTransaction:
+class AccountOperationRestrictionTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.ACCOUNT_OPERATION_RESTRICTION
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -8974,26 +13061,29 @@
 		'restriction_additions': 'array[TransactionType]',
 		'restriction_deletions': 'array[TransactionType]'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = AccountOperationRestrictionTransaction.TRANSACTION_VERSION
+		self._version = AccountOperationRestrictionTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = AccountOperationRestrictionTransaction.TRANSACTION_TYPE
+		self._type_ = AccountOperationRestrictionTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._restriction_flags = AccountRestrictionFlags.ADDRESS
 		self._restriction_additions = []
 		self._restriction_deletions = []
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._account_restriction_transaction_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -9088,15 +13178,15 @@
 		size += 1
 		size += 4
 		size += ArrayHelpers.size(self.restriction_additions)
 		size += ArrayHelpers.size(self.restriction_deletions)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> AccountOperationRestrictionTransaction:
+	def deserialize(cls, payload: ByteString) -> AccountOperationRestrictionTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -9128,15 +13218,15 @@
 		buffer = buffer[4:]
 		assert account_restriction_transaction_body_reserved_1 == 0, f'Invalid value of reserved field ({account_restriction_transaction_body_reserved_1})'
 		restriction_additions = ArrayHelpers.read_array_count(buffer, TransactionType, restriction_additions_count)
 		buffer = buffer[ArrayHelpers.size(restriction_additions):]
 		restriction_deletions = ArrayHelpers.read_array_count(buffer, TransactionType, restriction_deletions_count)
 		buffer = buffer[ArrayHelpers.size(restriction_deletions):]
 
-		instance = AccountOperationRestrictionTransaction()
+		instance = AccountOperationRestrictionTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -9177,38 +13267,41 @@
 		result += f'restriction_flags: {self._restriction_flags.__str__()}, '
 		result += f'restriction_additions: {list(map(str, self._restriction_additions))}, '
 		result += f'restriction_deletions: {list(map(str, self._restriction_deletions))}, '
 		result += ')'
 		return result
 
 
-class EmbeddedAccountOperationRestrictionTransaction:
+class EmbeddedAccountOperationRestrictionTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.ACCOUNT_OPERATION_RESTRICTION
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'restriction_flags': 'enum:AccountRestrictionFlags',
 		'restriction_additions': 'array[TransactionType]',
 		'restriction_deletions': 'array[TransactionType]'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedAccountOperationRestrictionTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedAccountOperationRestrictionTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedAccountOperationRestrictionTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedAccountOperationRestrictionTransactionV1.TRANSACTION_TYPE
 		self._restriction_flags = AccountRestrictionFlags.ADDRESS
 		self._restriction_additions = []
 		self._restriction_deletions = []
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._account_restriction_transaction_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -9276,15 +13369,15 @@
 		size += 1
 		size += 4
 		size += ArrayHelpers.size(self.restriction_additions)
 		size += ArrayHelpers.size(self.restriction_deletions)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedAccountOperationRestrictionTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedAccountOperationRestrictionTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -9310,15 +13403,15 @@
 		buffer = buffer[4:]
 		assert account_restriction_transaction_body_reserved_1 == 0, f'Invalid value of reserved field ({account_restriction_transaction_body_reserved_1})'
 		restriction_additions = ArrayHelpers.read_array_count(buffer, TransactionType, restriction_additions_count)
 		buffer = buffer[ArrayHelpers.size(restriction_additions):]
 		restriction_deletions = ArrayHelpers.read_array_count(buffer, TransactionType, restriction_deletions_count)
 		buffer = buffer[ArrayHelpers.size(restriction_deletions):]
 
-		instance = EmbeddedAccountOperationRestrictionTransaction()
+		instance = EmbeddedAccountOperationRestrictionTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._restriction_flags = restriction_flags
 		instance._restriction_additions = restriction_additions
 		instance._restriction_deletions = restriction_deletions
@@ -9350,15 +13443,15 @@
 		result += f'restriction_flags: {self._restriction_flags.__str__()}, '
 		result += f'restriction_additions: {list(map(str, self._restriction_additions))}, '
 		result += f'restriction_deletions: {list(map(str, self._restriction_deletions))}, '
 		result += ')'
 		return result
 
 
-class MosaicAddressRestrictionTransaction:
+class MosaicAddressRestrictionTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_ADDRESS_RESTRICTION
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -9367,27 +13460,30 @@
 		'mosaic_id': 'pod:UnresolvedMosaicId',
 		'target_address': 'pod:UnresolvedAddress'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = MosaicAddressRestrictionTransaction.TRANSACTION_VERSION
+		self._version = MosaicAddressRestrictionTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = MosaicAddressRestrictionTransaction.TRANSACTION_TYPE
+		self._type_ = MosaicAddressRestrictionTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._mosaic_id = UnresolvedMosaicId()
 		self._restriction_key = 0
 		self._previous_restriction_value = 0
 		self._new_restriction_value = 0
 		self._target_address = UnresolvedAddress()
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -9497,15 +13593,15 @@
 		size += 8
 		size += 8
 		size += 8
 		size += self.target_address.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> MosaicAddressRestrictionTransaction:
+	def deserialize(cls, payload: ByteString) -> MosaicAddressRestrictionTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -9534,15 +13630,15 @@
 		previous_restriction_value = int.from_bytes(buffer[:8], byteorder='little', signed=False)
 		buffer = buffer[8:]
 		new_restriction_value = int.from_bytes(buffer[:8], byteorder='little', signed=False)
 		buffer = buffer[8:]
 		target_address = UnresolvedAddress.deserialize(buffer)
 		buffer = buffer[target_address.size:]
 
-		instance = MosaicAddressRestrictionTransaction()
+		instance = MosaicAddressRestrictionTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -9586,38 +13682,41 @@
 		result += f'previous_restriction_value: 0x{self._previous_restriction_value:X}, '
 		result += f'new_restriction_value: 0x{self._new_restriction_value:X}, '
 		result += f'target_address: {self._target_address.__str__()}, '
 		result += ')'
 		return result
 
 
-class EmbeddedMosaicAddressRestrictionTransaction:
+class EmbeddedMosaicAddressRestrictionTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_ADDRESS_RESTRICTION
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'mosaic_id': 'pod:UnresolvedMosaicId',
 		'target_address': 'pod:UnresolvedAddress'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedMosaicAddressRestrictionTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedMosaicAddressRestrictionTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedMosaicAddressRestrictionTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedMosaicAddressRestrictionTransactionV1.TRANSACTION_TYPE
 		self._mosaic_id = UnresolvedMosaicId()
 		self._restriction_key = 0
 		self._previous_restriction_value = 0
 		self._new_restriction_value = 0
 		self._target_address = UnresolvedAddress()
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -9700,15 +13799,15 @@
 		size += 8
 		size += 8
 		size += 8
 		size += self.target_address.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedMosaicAddressRestrictionTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedMosaicAddressRestrictionTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -9731,15 +13830,15 @@
 		previous_restriction_value = int.from_bytes(buffer[:8], byteorder='little', signed=False)
 		buffer = buffer[8:]
 		new_restriction_value = int.from_bytes(buffer[:8], byteorder='little', signed=False)
 		buffer = buffer[8:]
 		target_address = UnresolvedAddress.deserialize(buffer)
 		buffer = buffer[target_address.size:]
 
-		instance = EmbeddedMosaicAddressRestrictionTransaction()
+		instance = EmbeddedMosaicAddressRestrictionTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._mosaic_id = mosaic_id
 		instance._restriction_key = restriction_key
 		instance._previous_restriction_value = previous_restriction_value
@@ -9813,15 +13912,15 @@
 
 	def serialize(self) -> bytes:
 		buffer = bytes()
 		buffer += self.value.to_bytes(1, byteorder='little', signed=False)
 		return buffer
 
 
-class MosaicGlobalRestrictionTransaction:
+class MosaicGlobalRestrictionTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_GLOBAL_RESTRICTION
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -9832,29 +13931,32 @@
 		'previous_restriction_type': 'enum:MosaicRestrictionType',
 		'new_restriction_type': 'enum:MosaicRestrictionType'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = MosaicGlobalRestrictionTransaction.TRANSACTION_VERSION
+		self._version = MosaicGlobalRestrictionTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = MosaicGlobalRestrictionTransaction.TRANSACTION_TYPE
+		self._type_ = MosaicGlobalRestrictionTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._mosaic_id = UnresolvedMosaicId()
 		self._reference_mosaic_id = UnresolvedMosaicId()
 		self._restriction_key = 0
 		self._previous_restriction_value = 0
 		self._new_restriction_value = 0
 		self._previous_restriction_type = MosaicRestrictionType.NONE
 		self._new_restriction_type = MosaicRestrictionType.NONE
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -9982,15 +14084,15 @@
 		size += 8
 		size += 8
 		size += self.previous_restriction_type.size
 		size += self.new_restriction_type.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> MosaicGlobalRestrictionTransaction:
+	def deserialize(cls, payload: ByteString) -> MosaicGlobalRestrictionTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -10023,15 +14125,15 @@
 		new_restriction_value = int.from_bytes(buffer[:8], byteorder='little', signed=False)
 		buffer = buffer[8:]
 		previous_restriction_type = MosaicRestrictionType.deserialize(buffer)
 		buffer = buffer[previous_restriction_type.size:]
 		new_restriction_type = MosaicRestrictionType.deserialize(buffer)
 		buffer = buffer[new_restriction_type.size:]
 
-		instance = MosaicGlobalRestrictionTransaction()
+		instance = MosaicGlobalRestrictionTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -10081,42 +14183,45 @@
 		result += f'new_restriction_value: 0x{self._new_restriction_value:X}, '
 		result += f'previous_restriction_type: {self._previous_restriction_type.__str__()}, '
 		result += f'new_restriction_type: {self._new_restriction_type.__str__()}, '
 		result += ')'
 		return result
 
 
-class EmbeddedMosaicGlobalRestrictionTransaction:
+class EmbeddedMosaicGlobalRestrictionTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.MOSAIC_GLOBAL_RESTRICTION
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'mosaic_id': 'pod:UnresolvedMosaicId',
 		'reference_mosaic_id': 'pod:UnresolvedMosaicId',
 		'previous_restriction_type': 'enum:MosaicRestrictionType',
 		'new_restriction_type': 'enum:MosaicRestrictionType'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedMosaicGlobalRestrictionTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedMosaicGlobalRestrictionTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedMosaicGlobalRestrictionTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedMosaicGlobalRestrictionTransactionV1.TRANSACTION_TYPE
 		self._mosaic_id = UnresolvedMosaicId()
 		self._reference_mosaic_id = UnresolvedMosaicId()
 		self._restriction_key = 0
 		self._previous_restriction_value = 0
 		self._new_restriction_value = 0
 		self._previous_restriction_type = MosaicRestrictionType.NONE
 		self._new_restriction_type = MosaicRestrictionType.NONE
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 
+	def sort(self) -> None:
+		pass
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -10217,15 +14322,15 @@
 		size += 8
 		size += 8
 		size += self.previous_restriction_type.size
 		size += self.new_restriction_type.size
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedMosaicGlobalRestrictionTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedMosaicGlobalRestrictionTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -10252,15 +14357,15 @@
 		new_restriction_value = int.from_bytes(buffer[:8], byteorder='little', signed=False)
 		buffer = buffer[8:]
 		previous_restriction_type = MosaicRestrictionType.deserialize(buffer)
 		buffer = buffer[previous_restriction_type.size:]
 		new_restriction_type = MosaicRestrictionType.deserialize(buffer)
 		buffer = buffer[new_restriction_type.size:]
 
-		instance = EmbeddedMosaicGlobalRestrictionTransaction()
+		instance = EmbeddedMosaicGlobalRestrictionTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._mosaic_id = mosaic_id
 		instance._reference_mosaic_id = reference_mosaic_id
 		instance._restriction_key = restriction_key
@@ -10301,15 +14406,15 @@
 		result += f'new_restriction_value: 0x{self._new_restriction_value:X}, '
 		result += f'previous_restriction_type: {self._previous_restriction_type.__str__()}, '
 		result += f'new_restriction_type: {self._new_restriction_type.__str__()}, '
 		result += ')'
 		return result
 
 
-class TransferTransaction:
+class TransferTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.TRANSFER
 	TYPE_HINTS = {
 		'signature': 'pod:Signature',
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
@@ -10319,27 +14424,30 @@
 		'mosaics': 'array[UnresolvedMosaic]',
 		'message': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._signature = Signature()
 		self._signer_public_key = PublicKey()
-		self._version = TransferTransaction.TRANSACTION_VERSION
+		self._version = TransferTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = TransferTransaction.TRANSACTION_TYPE
+		self._type_ = TransferTransactionV1.TRANSACTION_TYPE
 		self._fee = Amount()
 		self._deadline = Timestamp()
 		self._recipient_address = UnresolvedAddress()
 		self._mosaics = []
 		self._message = bytes()
 		self._verifiable_entity_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._transfer_transaction_body_reserved_1 = 0  # reserved field
 		self._transfer_transaction_body_reserved_2 = 0  # reserved field
 
+	def sort(self) -> None:
+		self._mosaics = sorted(self._mosaics, key=lambda e: e.mosaic_id.comparer() if hasattr(e.mosaic_id, 'comparer') else e.mosaic_id)
+
 	@property
 	def signature(self) -> Signature:
 		return self._signature
 
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
@@ -10435,15 +14543,15 @@
 		size += 1
 		size += 4
 		size += ArrayHelpers.size(self.mosaics)
 		size += len(self._message)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> TransferTransaction:
+	def deserialize(cls, payload: ByteString) -> TransferTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		verifiable_entity_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -10473,20 +14581,20 @@
 		buffer = buffer[1:]
 		transfer_transaction_body_reserved_1 = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		assert transfer_transaction_body_reserved_1 == 0, f'Invalid value of reserved field ({transfer_transaction_body_reserved_1})'
 		transfer_transaction_body_reserved_2 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		assert transfer_transaction_body_reserved_2 == 0, f'Invalid value of reserved field ({transfer_transaction_body_reserved_2})'
-		mosaics = ArrayHelpers.read_array_count(buffer, UnresolvedMosaic, mosaics_count, lambda e: e.mosaic_id)
+		mosaics = ArrayHelpers.read_array_count(buffer, UnresolvedMosaic, mosaics_count, lambda e: e.mosaic_id.comparer() if hasattr(e.mosaic_id, 'comparer') else e.mosaic_id)
 		buffer = buffer[ArrayHelpers.size(mosaics):]
 		message = ArrayHelpers.get_bytes(buffer, message_size)
 		buffer = buffer[message_size:]
 
-		instance = TransferTransaction()
+		instance = TransferTransactionV1()
 		instance._signature = signature
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._fee = fee
 		instance._deadline = deadline
@@ -10508,15 +14616,15 @@
 		buffer += self._fee.serialize()
 		buffer += self._deadline.serialize()
 		buffer += self._recipient_address.serialize()
 		buffer += len(self._message).to_bytes(2, byteorder='little', signed=False)  # message_size
 		buffer += len(self._mosaics).to_bytes(1, byteorder='little', signed=False)  # mosaics_count
 		buffer += self._transfer_transaction_body_reserved_1.to_bytes(1, byteorder='little', signed=False)
 		buffer += self._transfer_transaction_body_reserved_2.to_bytes(4, byteorder='little', signed=False)
-		buffer += ArrayHelpers.write_array(self._mosaics, lambda e: e.mosaic_id)
+		buffer += ArrayHelpers.write_array(self._mosaics, lambda e: e.mosaic_id.comparer() if hasattr(e.mosaic_id, 'comparer') else e.mosaic_id)
 		buffer += self._message
 		return buffer
 
 	def __str__(self) -> str:
 		result = '('
 		result += f'signature: {self._signature.__str__()}, '
 		result += f'signer_public_key: {self._signer_public_key.__str__()}, '
@@ -10528,39 +14636,42 @@
 		result += f'recipient_address: {self._recipient_address.__str__()}, '
 		result += f'mosaics: {list(map(str, self._mosaics))}, '
 		result += f'message: {hexlify(self._message).decode("utf8")}, '
 		result += ')'
 		return result
 
 
-class EmbeddedTransferTransaction:
+class EmbeddedTransferTransactionV1:
 	TRANSACTION_VERSION: int = 1
 	TRANSACTION_TYPE: TransactionType = TransactionType.TRANSFER
 	TYPE_HINTS = {
 		'signer_public_key': 'pod:PublicKey',
 		'network': 'enum:NetworkType',
 		'type_': 'enum:TransactionType',
 		'recipient_address': 'pod:UnresolvedAddress',
 		'mosaics': 'array[UnresolvedMosaic]',
 		'message': 'bytes_array'
 	}
 
 	def __init__(self):
 		self._signer_public_key = PublicKey()
-		self._version = EmbeddedTransferTransaction.TRANSACTION_VERSION
+		self._version = EmbeddedTransferTransactionV1.TRANSACTION_VERSION
 		self._network = NetworkType.MAINNET
-		self._type_ = EmbeddedTransferTransaction.TRANSACTION_TYPE
+		self._type_ = EmbeddedTransferTransactionV1.TRANSACTION_TYPE
 		self._recipient_address = UnresolvedAddress()
 		self._mosaics = []
 		self._message = bytes()
 		self._embedded_transaction_header_reserved_1 = 0  # reserved field
 		self._entity_body_reserved_1 = 0  # reserved field
 		self._transfer_transaction_body_reserved_1 = 0  # reserved field
 		self._transfer_transaction_body_reserved_2 = 0  # reserved field
 
+	def sort(self) -> None:
+		self._mosaics = sorted(self._mosaics, key=lambda e: e.mosaic_id.comparer() if hasattr(e.mosaic_id, 'comparer') else e.mosaic_id)
+
 	@property
 	def signer_public_key(self) -> PublicKey:
 		return self._signer_public_key
 
 	@property
 	def version(self) -> int:
 		return self._version
@@ -10629,15 +14740,15 @@
 		size += 1
 		size += 4
 		size += ArrayHelpers.size(self.mosaics)
 		size += len(self._message)
 		return size
 
 	@classmethod
-	def deserialize(cls, payload: ByteString) -> EmbeddedTransferTransaction:
+	def deserialize(cls, payload: ByteString) -> EmbeddedTransferTransactionV1:
 		buffer = memoryview(payload)
 		size_ = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		buffer = buffer[:size_ - 4]
 		del size_
 		embedded_transaction_header_reserved_1 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
@@ -10661,20 +14772,20 @@
 		buffer = buffer[1:]
 		transfer_transaction_body_reserved_1 = int.from_bytes(buffer[:1], byteorder='little', signed=False)
 		buffer = buffer[1:]
 		assert transfer_transaction_body_reserved_1 == 0, f'Invalid value of reserved field ({transfer_transaction_body_reserved_1})'
 		transfer_transaction_body_reserved_2 = int.from_bytes(buffer[:4], byteorder='little', signed=False)
 		buffer = buffer[4:]
 		assert transfer_transaction_body_reserved_2 == 0, f'Invalid value of reserved field ({transfer_transaction_body_reserved_2})'
-		mosaics = ArrayHelpers.read_array_count(buffer, UnresolvedMosaic, mosaics_count, lambda e: e.mosaic_id)
+		mosaics = ArrayHelpers.read_array_count(buffer, UnresolvedMosaic, mosaics_count, lambda e: e.mosaic_id.comparer() if hasattr(e.mosaic_id, 'comparer') else e.mosaic_id)
 		buffer = buffer[ArrayHelpers.size(mosaics):]
 		message = ArrayHelpers.get_bytes(buffer, message_size)
 		buffer = buffer[message_size:]
 
-		instance = EmbeddedTransferTransaction()
+		instance = EmbeddedTransferTransactionV1()
 		instance._signer_public_key = signer_public_key
 		instance._version = version
 		instance._network = network
 		instance._type_ = type_
 		instance._recipient_address = recipient_address
 		instance._mosaics = mosaics
 		instance._message = message
@@ -10690,15 +14801,15 @@
 		buffer += self._network.serialize()
 		buffer += self._type_.serialize()
 		buffer += self._recipient_address.serialize()
 		buffer += len(self._message).to_bytes(2, byteorder='little', signed=False)  # message_size
 		buffer += len(self._mosaics).to_bytes(1, byteorder='little', signed=False)  # mosaics_count
 		buffer += self._transfer_transaction_body_reserved_1.to_bytes(1, byteorder='little', signed=False)
 		buffer += self._transfer_transaction_body_reserved_2.to_bytes(4, byteorder='little', signed=False)
-		buffer += ArrayHelpers.write_array(self._mosaics, lambda e: e.mosaic_id)
+		buffer += ArrayHelpers.write_array(self._mosaics, lambda e: e.mosaic_id.comparer() if hasattr(e.mosaic_id, 'comparer') else e.mosaic_id)
 		buffer += self._message
 		return buffer
 
 	def __str__(self) -> str:
 		result = '('
 		result += f'signer_public_key: {self._signer_public_key.__str__()}, '
 		result += f'version: 0x{self._version:X}, '
@@ -10713,139 +14824,219 @@
 
 class TransactionFactory:
 	@classmethod
 	def deserialize(cls, payload: bytes) -> Transaction:
 		buffer = bytes(payload)
 		parent = Transaction.deserialize(buffer)
 		mapping = {
-			(AccountKeyLinkTransaction.TRANSACTION_TYPE): AccountKeyLinkTransaction,
-			(NodeKeyLinkTransaction.TRANSACTION_TYPE): NodeKeyLinkTransaction,
-			(AggregateCompleteTransaction.TRANSACTION_TYPE): AggregateCompleteTransaction,
-			(AggregateBondedTransaction.TRANSACTION_TYPE): AggregateBondedTransaction,
-			(VotingKeyLinkTransaction.TRANSACTION_TYPE): VotingKeyLinkTransaction,
-			(VrfKeyLinkTransaction.TRANSACTION_TYPE): VrfKeyLinkTransaction,
-			(HashLockTransaction.TRANSACTION_TYPE): HashLockTransaction,
-			(SecretLockTransaction.TRANSACTION_TYPE): SecretLockTransaction,
-			(SecretProofTransaction.TRANSACTION_TYPE): SecretProofTransaction,
-			(AccountMetadataTransaction.TRANSACTION_TYPE): AccountMetadataTransaction,
-			(MosaicMetadataTransaction.TRANSACTION_TYPE): MosaicMetadataTransaction,
-			(NamespaceMetadataTransaction.TRANSACTION_TYPE): NamespaceMetadataTransaction,
-			(MosaicDefinitionTransaction.TRANSACTION_TYPE): MosaicDefinitionTransaction,
-			(MosaicSupplyChangeTransaction.TRANSACTION_TYPE): MosaicSupplyChangeTransaction,
-			(MosaicSupplyRevocationTransaction.TRANSACTION_TYPE): MosaicSupplyRevocationTransaction,
-			(MultisigAccountModificationTransaction.TRANSACTION_TYPE): MultisigAccountModificationTransaction,
-			(AddressAliasTransaction.TRANSACTION_TYPE): AddressAliasTransaction,
-			(MosaicAliasTransaction.TRANSACTION_TYPE): MosaicAliasTransaction,
-			(NamespaceRegistrationTransaction.TRANSACTION_TYPE): NamespaceRegistrationTransaction,
-			(AccountAddressRestrictionTransaction.TRANSACTION_TYPE): AccountAddressRestrictionTransaction,
-			(AccountMosaicRestrictionTransaction.TRANSACTION_TYPE): AccountMosaicRestrictionTransaction,
-			(AccountOperationRestrictionTransaction.TRANSACTION_TYPE): AccountOperationRestrictionTransaction,
-			(MosaicAddressRestrictionTransaction.TRANSACTION_TYPE): MosaicAddressRestrictionTransaction,
-			(MosaicGlobalRestrictionTransaction.TRANSACTION_TYPE): MosaicGlobalRestrictionTransaction,
-			(TransferTransaction.TRANSACTION_TYPE): TransferTransaction
+			(AccountKeyLinkTransactionV1.TRANSACTION_TYPE, AccountKeyLinkTransactionV1.TRANSACTION_VERSION): AccountKeyLinkTransactionV1,
+			(NodeKeyLinkTransactionV1.TRANSACTION_TYPE, NodeKeyLinkTransactionV1.TRANSACTION_VERSION): NodeKeyLinkTransactionV1,
+			(AggregateCompleteTransactionV1.TRANSACTION_TYPE, AggregateCompleteTransactionV1.TRANSACTION_VERSION): AggregateCompleteTransactionV1,
+			(AggregateCompleteTransactionV2.TRANSACTION_TYPE, AggregateCompleteTransactionV2.TRANSACTION_VERSION): AggregateCompleteTransactionV2,
+			(AggregateBondedTransactionV1.TRANSACTION_TYPE, AggregateBondedTransactionV1.TRANSACTION_VERSION): AggregateBondedTransactionV1,
+			(AggregateBondedTransactionV2.TRANSACTION_TYPE, AggregateBondedTransactionV2.TRANSACTION_VERSION): AggregateBondedTransactionV2,
+			(VotingKeyLinkTransactionV1.TRANSACTION_TYPE, VotingKeyLinkTransactionV1.TRANSACTION_VERSION): VotingKeyLinkTransactionV1,
+			(VrfKeyLinkTransactionV1.TRANSACTION_TYPE, VrfKeyLinkTransactionV1.TRANSACTION_VERSION): VrfKeyLinkTransactionV1,
+			(HashLockTransactionV1.TRANSACTION_TYPE, HashLockTransactionV1.TRANSACTION_VERSION): HashLockTransactionV1,
+			(SecretLockTransactionV1.TRANSACTION_TYPE, SecretLockTransactionV1.TRANSACTION_VERSION): SecretLockTransactionV1,
+			(SecretProofTransactionV1.TRANSACTION_TYPE, SecretProofTransactionV1.TRANSACTION_VERSION): SecretProofTransactionV1,
+			(AccountMetadataTransactionV1.TRANSACTION_TYPE, AccountMetadataTransactionV1.TRANSACTION_VERSION): AccountMetadataTransactionV1,
+			(MosaicMetadataTransactionV1.TRANSACTION_TYPE, MosaicMetadataTransactionV1.TRANSACTION_VERSION): MosaicMetadataTransactionV1,
+			(NamespaceMetadataTransactionV1.TRANSACTION_TYPE, NamespaceMetadataTransactionV1.TRANSACTION_VERSION): NamespaceMetadataTransactionV1,
+			(MosaicDefinitionTransactionV1.TRANSACTION_TYPE, MosaicDefinitionTransactionV1.TRANSACTION_VERSION): MosaicDefinitionTransactionV1,
+			(MosaicSupplyChangeTransactionV1.TRANSACTION_TYPE, MosaicSupplyChangeTransactionV1.TRANSACTION_VERSION): MosaicSupplyChangeTransactionV1,
+			(MosaicSupplyRevocationTransactionV1.TRANSACTION_TYPE, MosaicSupplyRevocationTransactionV1.TRANSACTION_VERSION): MosaicSupplyRevocationTransactionV1,
+			(MultisigAccountModificationTransactionV1.TRANSACTION_TYPE, MultisigAccountModificationTransactionV1.TRANSACTION_VERSION): MultisigAccountModificationTransactionV1,
+			(AddressAliasTransactionV1.TRANSACTION_TYPE, AddressAliasTransactionV1.TRANSACTION_VERSION): AddressAliasTransactionV1,
+			(MosaicAliasTransactionV1.TRANSACTION_TYPE, MosaicAliasTransactionV1.TRANSACTION_VERSION): MosaicAliasTransactionV1,
+			(NamespaceRegistrationTransactionV1.TRANSACTION_TYPE, NamespaceRegistrationTransactionV1.TRANSACTION_VERSION): NamespaceRegistrationTransactionV1,
+			(AccountAddressRestrictionTransactionV1.TRANSACTION_TYPE, AccountAddressRestrictionTransactionV1.TRANSACTION_VERSION): AccountAddressRestrictionTransactionV1,
+			(AccountMosaicRestrictionTransactionV1.TRANSACTION_TYPE, AccountMosaicRestrictionTransactionV1.TRANSACTION_VERSION): AccountMosaicRestrictionTransactionV1,
+			(AccountOperationRestrictionTransactionV1.TRANSACTION_TYPE, AccountOperationRestrictionTransactionV1.TRANSACTION_VERSION): AccountOperationRestrictionTransactionV1,
+			(MosaicAddressRestrictionTransactionV1.TRANSACTION_TYPE, MosaicAddressRestrictionTransactionV1.TRANSACTION_VERSION): MosaicAddressRestrictionTransactionV1,
+			(MosaicGlobalRestrictionTransactionV1.TRANSACTION_TYPE, MosaicGlobalRestrictionTransactionV1.TRANSACTION_VERSION): MosaicGlobalRestrictionTransactionV1,
+			(TransferTransactionV1.TRANSACTION_TYPE, TransferTransactionV1.TRANSACTION_VERSION): TransferTransactionV1
 		}
-		discriminator = (parent.type_)
+		discriminator = (parent.type_, parent.version)
 		factory_class = mapping[discriminator]
 		return factory_class.deserialize(buffer)
 
 	@classmethod
 	def create_by_name(cls, entity_name: str) -> Transaction:
 		mapping = {
-			'account_key_link_transaction': AccountKeyLinkTransaction,
-			'node_key_link_transaction': NodeKeyLinkTransaction,
-			'aggregate_complete_transaction': AggregateCompleteTransaction,
-			'aggregate_bonded_transaction': AggregateBondedTransaction,
-			'voting_key_link_transaction': VotingKeyLinkTransaction,
-			'vrf_key_link_transaction': VrfKeyLinkTransaction,
-			'hash_lock_transaction': HashLockTransaction,
-			'secret_lock_transaction': SecretLockTransaction,
-			'secret_proof_transaction': SecretProofTransaction,
-			'account_metadata_transaction': AccountMetadataTransaction,
-			'mosaic_metadata_transaction': MosaicMetadataTransaction,
-			'namespace_metadata_transaction': NamespaceMetadataTransaction,
-			'mosaic_definition_transaction': MosaicDefinitionTransaction,
-			'mosaic_supply_change_transaction': MosaicSupplyChangeTransaction,
-			'mosaic_supply_revocation_transaction': MosaicSupplyRevocationTransaction,
-			'multisig_account_modification_transaction': MultisigAccountModificationTransaction,
-			'address_alias_transaction': AddressAliasTransaction,
-			'mosaic_alias_transaction': MosaicAliasTransaction,
-			'namespace_registration_transaction': NamespaceRegistrationTransaction,
-			'account_address_restriction_transaction': AccountAddressRestrictionTransaction,
-			'account_mosaic_restriction_transaction': AccountMosaicRestrictionTransaction,
-			'account_operation_restriction_transaction': AccountOperationRestrictionTransaction,
-			'mosaic_address_restriction_transaction': MosaicAddressRestrictionTransaction,
-			'mosaic_global_restriction_transaction': MosaicGlobalRestrictionTransaction,
-			'transfer_transaction': TransferTransaction
+			'account_key_link_transaction_v1': AccountKeyLinkTransactionV1,
+			'node_key_link_transaction_v1': NodeKeyLinkTransactionV1,
+			'aggregate_complete_transaction_v1': AggregateCompleteTransactionV1,
+			'aggregate_complete_transaction_v2': AggregateCompleteTransactionV2,
+			'aggregate_bonded_transaction_v1': AggregateBondedTransactionV1,
+			'aggregate_bonded_transaction_v2': AggregateBondedTransactionV2,
+			'voting_key_link_transaction_v1': VotingKeyLinkTransactionV1,
+			'vrf_key_link_transaction_v1': VrfKeyLinkTransactionV1,
+			'hash_lock_transaction_v1': HashLockTransactionV1,
+			'secret_lock_transaction_v1': SecretLockTransactionV1,
+			'secret_proof_transaction_v1': SecretProofTransactionV1,
+			'account_metadata_transaction_v1': AccountMetadataTransactionV1,
+			'mosaic_metadata_transaction_v1': MosaicMetadataTransactionV1,
+			'namespace_metadata_transaction_v1': NamespaceMetadataTransactionV1,
+			'mosaic_definition_transaction_v1': MosaicDefinitionTransactionV1,
+			'mosaic_supply_change_transaction_v1': MosaicSupplyChangeTransactionV1,
+			'mosaic_supply_revocation_transaction_v1': MosaicSupplyRevocationTransactionV1,
+			'multisig_account_modification_transaction_v1': MultisigAccountModificationTransactionV1,
+			'address_alias_transaction_v1': AddressAliasTransactionV1,
+			'mosaic_alias_transaction_v1': MosaicAliasTransactionV1,
+			'namespace_registration_transaction_v1': NamespaceRegistrationTransactionV1,
+			'account_address_restriction_transaction_v1': AccountAddressRestrictionTransactionV1,
+			'account_mosaic_restriction_transaction_v1': AccountMosaicRestrictionTransactionV1,
+			'account_operation_restriction_transaction_v1': AccountOperationRestrictionTransactionV1,
+			'mosaic_address_restriction_transaction_v1': MosaicAddressRestrictionTransactionV1,
+			'mosaic_global_restriction_transaction_v1': MosaicGlobalRestrictionTransactionV1,
+			'transfer_transaction_v1': TransferTransactionV1
 		}
 
 		if entity_name not in mapping:
-			raise ValueError('unknown Transaction type')
+			raise ValueError(f'unknown Transaction type {entity_name}')
 
 		return mapping[entity_name]()
 
 
 class EmbeddedTransactionFactory:
 	@classmethod
 	def deserialize(cls, payload: bytes) -> EmbeddedTransaction:
 		buffer = bytes(payload)
 		parent = EmbeddedTransaction.deserialize(buffer)
 		mapping = {
-			(EmbeddedAccountKeyLinkTransaction.TRANSACTION_TYPE): EmbeddedAccountKeyLinkTransaction,
-			(EmbeddedNodeKeyLinkTransaction.TRANSACTION_TYPE): EmbeddedNodeKeyLinkTransaction,
-			(EmbeddedVotingKeyLinkTransaction.TRANSACTION_TYPE): EmbeddedVotingKeyLinkTransaction,
-			(EmbeddedVrfKeyLinkTransaction.TRANSACTION_TYPE): EmbeddedVrfKeyLinkTransaction,
-			(EmbeddedHashLockTransaction.TRANSACTION_TYPE): EmbeddedHashLockTransaction,
-			(EmbeddedSecretLockTransaction.TRANSACTION_TYPE): EmbeddedSecretLockTransaction,
-			(EmbeddedSecretProofTransaction.TRANSACTION_TYPE): EmbeddedSecretProofTransaction,
-			(EmbeddedAccountMetadataTransaction.TRANSACTION_TYPE): EmbeddedAccountMetadataTransaction,
-			(EmbeddedMosaicMetadataTransaction.TRANSACTION_TYPE): EmbeddedMosaicMetadataTransaction,
-			(EmbeddedNamespaceMetadataTransaction.TRANSACTION_TYPE): EmbeddedNamespaceMetadataTransaction,
-			(EmbeddedMosaicDefinitionTransaction.TRANSACTION_TYPE): EmbeddedMosaicDefinitionTransaction,
-			(EmbeddedMosaicSupplyChangeTransaction.TRANSACTION_TYPE): EmbeddedMosaicSupplyChangeTransaction,
-			(EmbeddedMosaicSupplyRevocationTransaction.TRANSACTION_TYPE): EmbeddedMosaicSupplyRevocationTransaction,
-			(EmbeddedMultisigAccountModificationTransaction.TRANSACTION_TYPE): EmbeddedMultisigAccountModificationTransaction,
-			(EmbeddedAddressAliasTransaction.TRANSACTION_TYPE): EmbeddedAddressAliasTransaction,
-			(EmbeddedMosaicAliasTransaction.TRANSACTION_TYPE): EmbeddedMosaicAliasTransaction,
-			(EmbeddedNamespaceRegistrationTransaction.TRANSACTION_TYPE): EmbeddedNamespaceRegistrationTransaction,
-			(EmbeddedAccountAddressRestrictionTransaction.TRANSACTION_TYPE): EmbeddedAccountAddressRestrictionTransaction,
-			(EmbeddedAccountMosaicRestrictionTransaction.TRANSACTION_TYPE): EmbeddedAccountMosaicRestrictionTransaction,
-			(EmbeddedAccountOperationRestrictionTransaction.TRANSACTION_TYPE): EmbeddedAccountOperationRestrictionTransaction,
-			(EmbeddedMosaicAddressRestrictionTransaction.TRANSACTION_TYPE): EmbeddedMosaicAddressRestrictionTransaction,
-			(EmbeddedMosaicGlobalRestrictionTransaction.TRANSACTION_TYPE): EmbeddedMosaicGlobalRestrictionTransaction,
-			(EmbeddedTransferTransaction.TRANSACTION_TYPE): EmbeddedTransferTransaction
+			(EmbeddedAccountKeyLinkTransactionV1.TRANSACTION_TYPE, EmbeddedAccountKeyLinkTransactionV1.TRANSACTION_VERSION): EmbeddedAccountKeyLinkTransactionV1,
+			(EmbeddedNodeKeyLinkTransactionV1.TRANSACTION_TYPE, EmbeddedNodeKeyLinkTransactionV1.TRANSACTION_VERSION): EmbeddedNodeKeyLinkTransactionV1,
+			(EmbeddedVotingKeyLinkTransactionV1.TRANSACTION_TYPE, EmbeddedVotingKeyLinkTransactionV1.TRANSACTION_VERSION): EmbeddedVotingKeyLinkTransactionV1,
+			(EmbeddedVrfKeyLinkTransactionV1.TRANSACTION_TYPE, EmbeddedVrfKeyLinkTransactionV1.TRANSACTION_VERSION): EmbeddedVrfKeyLinkTransactionV1,
+			(EmbeddedHashLockTransactionV1.TRANSACTION_TYPE, EmbeddedHashLockTransactionV1.TRANSACTION_VERSION): EmbeddedHashLockTransactionV1,
+			(EmbeddedSecretLockTransactionV1.TRANSACTION_TYPE, EmbeddedSecretLockTransactionV1.TRANSACTION_VERSION): EmbeddedSecretLockTransactionV1,
+			(EmbeddedSecretProofTransactionV1.TRANSACTION_TYPE, EmbeddedSecretProofTransactionV1.TRANSACTION_VERSION): EmbeddedSecretProofTransactionV1,
+			(EmbeddedAccountMetadataTransactionV1.TRANSACTION_TYPE, EmbeddedAccountMetadataTransactionV1.TRANSACTION_VERSION): EmbeddedAccountMetadataTransactionV1,
+			(EmbeddedMosaicMetadataTransactionV1.TRANSACTION_TYPE, EmbeddedMosaicMetadataTransactionV1.TRANSACTION_VERSION): EmbeddedMosaicMetadataTransactionV1,
+			(EmbeddedNamespaceMetadataTransactionV1.TRANSACTION_TYPE, EmbeddedNamespaceMetadataTransactionV1.TRANSACTION_VERSION): EmbeddedNamespaceMetadataTransactionV1,
+			(EmbeddedMosaicDefinitionTransactionV1.TRANSACTION_TYPE, EmbeddedMosaicDefinitionTransactionV1.TRANSACTION_VERSION): EmbeddedMosaicDefinitionTransactionV1,
+			(EmbeddedMosaicSupplyChangeTransactionV1.TRANSACTION_TYPE, EmbeddedMosaicSupplyChangeTransactionV1.TRANSACTION_VERSION): EmbeddedMosaicSupplyChangeTransactionV1,
+			(EmbeddedMosaicSupplyRevocationTransactionV1.TRANSACTION_TYPE, EmbeddedMosaicSupplyRevocationTransactionV1.TRANSACTION_VERSION): EmbeddedMosaicSupplyRevocationTransactionV1,
+			(EmbeddedMultisigAccountModificationTransactionV1.TRANSACTION_TYPE, EmbeddedMultisigAccountModificationTransactionV1.TRANSACTION_VERSION): EmbeddedMultisigAccountModificationTransactionV1,
+			(EmbeddedAddressAliasTransactionV1.TRANSACTION_TYPE, EmbeddedAddressAliasTransactionV1.TRANSACTION_VERSION): EmbeddedAddressAliasTransactionV1,
+			(EmbeddedMosaicAliasTransactionV1.TRANSACTION_TYPE, EmbeddedMosaicAliasTransactionV1.TRANSACTION_VERSION): EmbeddedMosaicAliasTransactionV1,
+			(EmbeddedNamespaceRegistrationTransactionV1.TRANSACTION_TYPE, EmbeddedNamespaceRegistrationTransactionV1.TRANSACTION_VERSION): EmbeddedNamespaceRegistrationTransactionV1,
+			(EmbeddedAccountAddressRestrictionTransactionV1.TRANSACTION_TYPE, EmbeddedAccountAddressRestrictionTransactionV1.TRANSACTION_VERSION): EmbeddedAccountAddressRestrictionTransactionV1,
+			(EmbeddedAccountMosaicRestrictionTransactionV1.TRANSACTION_TYPE, EmbeddedAccountMosaicRestrictionTransactionV1.TRANSACTION_VERSION): EmbeddedAccountMosaicRestrictionTransactionV1,
+			(EmbeddedAccountOperationRestrictionTransactionV1.TRANSACTION_TYPE, EmbeddedAccountOperationRestrictionTransactionV1.TRANSACTION_VERSION): EmbeddedAccountOperationRestrictionTransactionV1,
+			(EmbeddedMosaicAddressRestrictionTransactionV1.TRANSACTION_TYPE, EmbeddedMosaicAddressRestrictionTransactionV1.TRANSACTION_VERSION): EmbeddedMosaicAddressRestrictionTransactionV1,
+			(EmbeddedMosaicGlobalRestrictionTransactionV1.TRANSACTION_TYPE, EmbeddedMosaicGlobalRestrictionTransactionV1.TRANSACTION_VERSION): EmbeddedMosaicGlobalRestrictionTransactionV1,
+			(EmbeddedTransferTransactionV1.TRANSACTION_TYPE, EmbeddedTransferTransactionV1.TRANSACTION_VERSION): EmbeddedTransferTransactionV1
 		}
-		discriminator = (parent.type_)
+		discriminator = (parent.type_, parent.version)
 		factory_class = mapping[discriminator]
 		return factory_class.deserialize(buffer)
 
 	@classmethod
 	def create_by_name(cls, entity_name: str) -> EmbeddedTransaction:
 		mapping = {
-			'account_key_link_transaction': EmbeddedAccountKeyLinkTransaction,
-			'node_key_link_transaction': EmbeddedNodeKeyLinkTransaction,
-			'voting_key_link_transaction': EmbeddedVotingKeyLinkTransaction,
-			'vrf_key_link_transaction': EmbeddedVrfKeyLinkTransaction,
-			'hash_lock_transaction': EmbeddedHashLockTransaction,
-			'secret_lock_transaction': EmbeddedSecretLockTransaction,
-			'secret_proof_transaction': EmbeddedSecretProofTransaction,
-			'account_metadata_transaction': EmbeddedAccountMetadataTransaction,
-			'mosaic_metadata_transaction': EmbeddedMosaicMetadataTransaction,
-			'namespace_metadata_transaction': EmbeddedNamespaceMetadataTransaction,
-			'mosaic_definition_transaction': EmbeddedMosaicDefinitionTransaction,
-			'mosaic_supply_change_transaction': EmbeddedMosaicSupplyChangeTransaction,
-			'mosaic_supply_revocation_transaction': EmbeddedMosaicSupplyRevocationTransaction,
-			'multisig_account_modification_transaction': EmbeddedMultisigAccountModificationTransaction,
-			'address_alias_transaction': EmbeddedAddressAliasTransaction,
-			'mosaic_alias_transaction': EmbeddedMosaicAliasTransaction,
-			'namespace_registration_transaction': EmbeddedNamespaceRegistrationTransaction,
-			'account_address_restriction_transaction': EmbeddedAccountAddressRestrictionTransaction,
-			'account_mosaic_restriction_transaction': EmbeddedAccountMosaicRestrictionTransaction,
-			'account_operation_restriction_transaction': EmbeddedAccountOperationRestrictionTransaction,
-			'mosaic_address_restriction_transaction': EmbeddedMosaicAddressRestrictionTransaction,
-			'mosaic_global_restriction_transaction': EmbeddedMosaicGlobalRestrictionTransaction,
-			'transfer_transaction': EmbeddedTransferTransaction
+			'account_key_link_transaction_v1': EmbeddedAccountKeyLinkTransactionV1,
+			'node_key_link_transaction_v1': EmbeddedNodeKeyLinkTransactionV1,
+			'voting_key_link_transaction_v1': EmbeddedVotingKeyLinkTransactionV1,
+			'vrf_key_link_transaction_v1': EmbeddedVrfKeyLinkTransactionV1,
+			'hash_lock_transaction_v1': EmbeddedHashLockTransactionV1,
+			'secret_lock_transaction_v1': EmbeddedSecretLockTransactionV1,
+			'secret_proof_transaction_v1': EmbeddedSecretProofTransactionV1,
+			'account_metadata_transaction_v1': EmbeddedAccountMetadataTransactionV1,
+			'mosaic_metadata_transaction_v1': EmbeddedMosaicMetadataTransactionV1,
+			'namespace_metadata_transaction_v1': EmbeddedNamespaceMetadataTransactionV1,
+			'mosaic_definition_transaction_v1': EmbeddedMosaicDefinitionTransactionV1,
+			'mosaic_supply_change_transaction_v1': EmbeddedMosaicSupplyChangeTransactionV1,
+			'mosaic_supply_revocation_transaction_v1': EmbeddedMosaicSupplyRevocationTransactionV1,
+			'multisig_account_modification_transaction_v1': EmbeddedMultisigAccountModificationTransactionV1,
+			'address_alias_transaction_v1': EmbeddedAddressAliasTransactionV1,
+			'mosaic_alias_transaction_v1': EmbeddedMosaicAliasTransactionV1,
+			'namespace_registration_transaction_v1': EmbeddedNamespaceRegistrationTransactionV1,
+			'account_address_restriction_transaction_v1': EmbeddedAccountAddressRestrictionTransactionV1,
+			'account_mosaic_restriction_transaction_v1': EmbeddedAccountMosaicRestrictionTransactionV1,
+			'account_operation_restriction_transaction_v1': EmbeddedAccountOperationRestrictionTransactionV1,
+			'mosaic_address_restriction_transaction_v1': EmbeddedMosaicAddressRestrictionTransactionV1,
+			'mosaic_global_restriction_transaction_v1': EmbeddedMosaicGlobalRestrictionTransactionV1,
+			'transfer_transaction_v1': EmbeddedTransferTransactionV1
+		}
+
+		if entity_name not in mapping:
+			raise ValueError(f'unknown EmbeddedTransaction type {entity_name}')
+
+		return mapping[entity_name]()
+
+
+class BlockFactory:
+	@classmethod
+	def deserialize(cls, payload: bytes) -> Block:
+		buffer = bytes(payload)
+		parent = Block.deserialize(buffer)
+		mapping = {
+			(NemesisBlockV1.BLOCK_TYPE): NemesisBlockV1,
+			(NormalBlockV1.BLOCK_TYPE): NormalBlockV1,
+			(ImportanceBlockV1.BLOCK_TYPE): ImportanceBlockV1
+		}
+		discriminator = (parent.type_)
+		factory_class = mapping[discriminator]
+		return factory_class.deserialize(buffer)
+
+	@classmethod
+	def create_by_name(cls, entity_name: str) -> Block:
+		mapping = {
+			'nemesis_block_v1': NemesisBlockV1,
+			'normal_block_v1': NormalBlockV1,
+			'importance_block_v1': ImportanceBlockV1
+		}
+
+		if entity_name not in mapping:
+			raise ValueError(f'unknown Block type {entity_name}')
+
+		return mapping[entity_name]()
+
+
+class ReceiptFactory:
+	@classmethod
+	def deserialize(cls, payload: bytes) -> Receipt:
+		buffer = bytes(payload)
+		parent = Receipt.deserialize(buffer)
+		mapping = {
+			(HarvestFeeReceipt.RECEIPT_TYPE): HarvestFeeReceipt,
+			(InflationReceipt.RECEIPT_TYPE): InflationReceipt,
+			(LockHashCreatedFeeReceipt.RECEIPT_TYPE): LockHashCreatedFeeReceipt,
+			(LockHashCompletedFeeReceipt.RECEIPT_TYPE): LockHashCompletedFeeReceipt,
+			(LockHashExpiredFeeReceipt.RECEIPT_TYPE): LockHashExpiredFeeReceipt,
+			(LockSecretCreatedFeeReceipt.RECEIPT_TYPE): LockSecretCreatedFeeReceipt,
+			(LockSecretCompletedFeeReceipt.RECEIPT_TYPE): LockSecretCompletedFeeReceipt,
+			(LockSecretExpiredFeeReceipt.RECEIPT_TYPE): LockSecretExpiredFeeReceipt,
+			(MosaicExpiredReceipt.RECEIPT_TYPE): MosaicExpiredReceipt,
+			(MosaicRentalFeeReceipt.RECEIPT_TYPE): MosaicRentalFeeReceipt,
+			(NamespaceExpiredReceipt.RECEIPT_TYPE): NamespaceExpiredReceipt,
+			(NamespaceDeletedReceipt.RECEIPT_TYPE): NamespaceDeletedReceipt,
+			(NamespaceRentalFeeReceipt.RECEIPT_TYPE): NamespaceRentalFeeReceipt
+		}
+		discriminator = (parent.type_)
+		factory_class = mapping[discriminator]
+		return factory_class.deserialize(buffer)
+
+	@classmethod
+	def create_by_name(cls, entity_name: str) -> Receipt:
+		mapping = {
+			'harvest_fee_receipt': HarvestFeeReceipt,
+			'inflation_receipt': InflationReceipt,
+			'lock_hash_created_fee_receipt': LockHashCreatedFeeReceipt,
+			'lock_hash_completed_fee_receipt': LockHashCompletedFeeReceipt,
+			'lock_hash_expired_fee_receipt': LockHashExpiredFeeReceipt,
+			'lock_secret_created_fee_receipt': LockSecretCreatedFeeReceipt,
+			'lock_secret_completed_fee_receipt': LockSecretCompletedFeeReceipt,
+			'lock_secret_expired_fee_receipt': LockSecretExpiredFeeReceipt,
+			'mosaic_expired_receipt': MosaicExpiredReceipt,
+			'mosaic_rental_fee_receipt': MosaicRentalFeeReceipt,
+			'namespace_expired_receipt': NamespaceExpiredReceipt,
+			'namespace_deleted_receipt': NamespaceDeletedReceipt,
+			'namespace_rental_fee_receipt': NamespaceRentalFeeReceipt
 		}
 
 		if entity_name not in mapping:
-			raise ValueError('unknown EmbeddedTransaction type')
+			raise ValueError(f'unknown Receipt type {entity_name}')
 
 		return mapping[entity_name]()
```

### Comparing `symbol-sdk-python-3.0.3/symbolchain/symbol/IdGenerator.py` & `symbol-sdk-python-3.0.5/symbolchain/symbol/IdGenerator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import sha3
+import hashlib
 
 NAMESPACE_FLAG = 1 << 63
 
 
 def generate_mosaic_id(owner_address, nonce):
 	"""Generates a mosaic id from an owner address and a nonce."""
-	hasher = sha3.sha3_256()
+	hasher = hashlib.sha3_256()
 	hasher.update(nonce.to_bytes(4, 'little'))
 	hasher.update(owner_address.bytes)
 	digest = hasher.digest()
 
 	result = int.from_bytes(digest[0:8], 'little')
 	if result & NAMESPACE_FLAG:
 		result -= NAMESPACE_FLAG
 
 	return result
 
 
 def generate_namespace_id(name, parent_namespace_id=0):
 	"""Generates a namespace id from a name and an optional parent namespace id."""
-	hasher = sha3.sha3_256()
+	hasher = hashlib.sha3_256()
 	hasher.update(parent_namespace_id.to_bytes(8, 'little'))
 	hasher.update(name.encode('utf8'))
 	digest = hasher.digest()
 
 	result = int.from_bytes(digest[0:8], 'little')
 	return result | NAMESPACE_FLAG
```

### Comparing `symbol-sdk-python-3.0.3/symbolchain/symbol/Network.py` & `symbol-sdk-python-3.0.5/symbolchain/symbol/Network.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,71 @@
 import base64
-
-import sha3
+import datetime
+import hashlib
 
 from ..ByteArray import ByteArray
 from ..CryptoTypes import Hash256
 from ..Network import Network as BasicNetwork
+from ..NetworkTimestamp import NetworkTimestamp as BasicNetworkTimestamp
+from ..NetworkTimestamp import NetworkTimestampDatetimeConverter
+
+
+class NetworkTimestamp(BasicNetworkTimestamp):
+	"""Represents a symbol network timestamp with millisecond resolution."""
+
+	def add_milliseconds(self, count):
+		"""Adds a specified number of milliseconds to this timestamp."""
+		return NetworkTimestamp(self.timestamp + count)
+
+	def add_seconds(self, count):
+		return self.add_milliseconds(1000 * count)
 
 
 class Address(ByteArray):
 	"""Represents a Symbol address."""
 
 	SIZE = 24
+	ENCODED_SIZE = 39
 
 	def __init__(self, address):
 		"""Creates an address from a decoded or encoded address."""
 		raw_bytes = address
 		if isinstance(address, str):
 			raw_bytes = base64.b32decode(address + 'A')[0:-1]
 		elif isinstance(address, Address):
 			raw_bytes = address.bytes
 
 		super().__init__(self.SIZE, raw_bytes, Address)
 
 	def __str__(self):
 		return base64.b32encode(self.bytes + bytes(0)).decode('utf8')[0:-1]
 
+	def __repr__(self):
+		return f'Address(\'{str(self)}\')'
+
 
 class Network(BasicNetwork):
 	"""Represents a Symbol network."""
 
-	def __init__(self, name, identifier, generation_hash_seed=None):
-		"""Creates a new network with the specified name, identifier byte and generation hash seed."""
-		super().__init__(name, identifier)
+	def __init__(self, name, identifier, epoch_time, generation_hash_seed=None):
+		"""Creates a new network with the specified properties."""
+		super().__init__(name, identifier, NetworkTimestampDatetimeConverter(epoch_time, 'milliseconds'), Address, NetworkTimestamp)
 		self.generation_hash_seed = generation_hash_seed
 
 	def address_hasher(self):
-		return sha3.sha3_256()
+		return hashlib.sha3_256()
 
 	def create_address(self, address_without_checksum, checksum):
 		return Address(address_without_checksum + checksum[0:3])
 
 
-Network.MAINNET = Network('mainnet', 0x68, Hash256('57F7DA205008026C776CB6AED843393F04CD458E0AA2D9F1D5F31A402072B2D6'))
-Network.TESTNET = Network('testnet', 0x98, Hash256('7FCCD304802016BEBBCD342A332F91FF1F3BB5E902988B352697BE245F48E836'))
+Network.MAINNET = Network(
+	'mainnet',
+	0x68,
+	datetime.datetime(2021, 3, 16, 0, 6, 25, tzinfo=datetime.timezone.utc),
+	Hash256('57F7DA205008026C776CB6AED843393F04CD458E0AA2D9F1D5F31A402072B2D6'))
+Network.TESTNET = Network(
+	'testnet',
+	0x98,
+	datetime.datetime(2022, 10, 31, 21, 7, 47, tzinfo=datetime.timezone.utc),
+	Hash256('49D6E1CE276A85B70EAFE52349AACCA389302E7A9754BCF1221E79494FC665A4'))
 Network.NETWORKS = [Network.MAINNET, Network.TESTNET]
```

### Comparing `symbol-sdk-python-3.0.3/setup.py` & `symbol-sdk-python-3.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['symbolchain',
+ 'symbolchain.external',
  'symbolchain.facade',
+ 'symbolchain.impl',
  'symbolchain.nc',
  'symbolchain.nem',
- 'symbolchain.nem.external',
  'symbolchain.sc',
  'symbolchain.symbol']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Pillow==9.0.1',
+['Pillow==9.5.0',
+ 'PyNaCl==1.5.0',
  'PyYAML==6.0',
- 'cryptography==36.0.1',
+ 'cryptography==40.0.1',
  'mnemonic==0.20',
- 'pysha3==1.0.2',
- 'pyzbar==0.1.8',
- 'qrcode==7.3.1']
+ 'pyzbar==0.1.9',
+ 'qrcode==7.4.2',
+ 'ripemd-hash==1.0.0',
+ 'safe-pysha3==1.0.3']
 
 setup_kwargs = {
     'name': 'symbol-sdk-python',
-    'version': '3.0.3',
+    'version': '3.0.5',
     'description': 'Symbol SDK',
     'long_description': '# Symbol-sdk-core-python\n\n[![Build Status](https://travis-ci.com/nemtech/symbol-sdk-core-python.svg?branch=main)](https://travis-ci.com/nemtech/symbol-sdk-core-python)\n[![PyPI version](https://img.shields.io/pypi/v/symbol-sdk-core-python.svg)](https://pypi.python.org/pypi/symbol-sdk-core-python/)\n\nThis is symbol project core sdk python library.\n',
     'author': 'Symbol Contributors',
     'author_email': 'contributors@symbol.dev',
     'maintainer': 'Symbol Contributors',
     'maintainer_email': 'contributors@symbol.dev',
     'url': 'https://github.com/symbol/symbol/tree/main/sdk/python',
```

### Comparing `symbol-sdk-python-3.0.3/PKG-INFO` & `symbol-sdk-python-3.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbol-sdk-python
-Version: 3.0.3
+Version: 3.0.5
 Summary: Symbol SDK
 Home-page: https://github.com/symbol/symbol/tree/main/sdk/python
 License: MIT
 Keywords: symbol,sdk,Symbol SDK
 Author: Symbol Contributors
 Author-email: contributors@symbol.dev
 Maintainer: Symbol Contributors
@@ -12,21 +12,23 @@
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Pillow (==9.0.1)
+Requires-Dist: Pillow (==9.5.0)
+Requires-Dist: PyNaCl (==1.5.0)
 Requires-Dist: PyYAML (==6.0)
-Requires-Dist: cryptography (==36.0.1)
+Requires-Dist: cryptography (==40.0.1)
 Requires-Dist: mnemonic (==0.20)
-Requires-Dist: pysha3 (==1.0.2)
-Requires-Dist: pyzbar (==0.1.8)
-Requires-Dist: qrcode (==7.3.1)
+Requires-Dist: pyzbar (==0.1.9)
+Requires-Dist: qrcode (==7.4.2)
+Requires-Dist: ripemd-hash (==1.0.0)
+Requires-Dist: safe-pysha3 (==1.0.3)
 Project-URL: Repository, https://github.com/symbol/symbol/tree/main/sdk/python
 Description-Content-Type: text/markdown
 
 # Symbol-sdk-core-python
 
 [![Build Status](https://travis-ci.com/nemtech/symbol-sdk-core-python.svg?branch=main)](https://travis-ci.com/nemtech/symbol-sdk-core-python)
 [![PyPI version](https://img.shields.io/pypi/v/symbol-sdk-core-python.svg)](https://pypi.python.org/pypi/symbol-sdk-core-python/)
```

