# Comparing `tmp/pytest_evm-0.1.1.tar.gz` & `tmp/pytest_evm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_evm-0.1.1.tar", max compression
+gzip compressed data, was "pytest_evm-0.1.2.tar", max compression
```

## Comparing `pytest_evm-0.1.1.tar` & `pytest_evm-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1063 2024-01-24 19:16:03.258573 pytest_evm-0.1.1/LICENSE
--rw-r--r--   0        0        0     4209 2024-01-24 19:16:03.261582 pytest_evm-0.1.1/README.md
--rw-r--r--   0        0        0     1448 2024-04-17 17:37:09.523443 pytest_evm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      192 2024-01-24 18:08:51.851477 pytest_evm-0.1.1/pytest_evm/__init__.py
--rw-r--r--   0        0        0      759 2024-01-24 18:35:25.074374 pytest_evm-0.1.1/pytest_evm/fixtures.py
--rw-r--r--   0        0        0     1956 2024-04-17 17:38:49.298623 pytest_evm-0.1.1/pytest_evm/hooks.py
--rw-r--r--   0        0        0       62 2023-12-04 17:21:05.182141 pytest_evm-0.1.1/pytest_evm/pytest.ini
--rw-r--r--   0        0        0     1859 2024-04-17 17:31:49.858690 pytest_evm-0.1.1/pytest_evm/utils.py
--rw-r--r--   0        0        0     5437 1970-01-01 00:00:00.000000 pytest_evm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-01-24 19:16:03.258573 pytest_evm-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4283 2024-04-20 09:59:38.539266 pytest_evm-0.1.2/README.md
+-rw-r--r--   0        0        0     1448 2024-04-20 10:07:28.234886 pytest_evm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      192 2024-01-24 18:08:51.851477 pytest_evm-0.1.2/pytest_evm/__init__.py
+-rw-r--r--   0        0        0      295 2024-04-20 09:57:52.917480 pytest_evm-0.1.2/pytest_evm/exceptions.py
+-rw-r--r--   0        0        0      759 2024-01-24 18:35:25.074374 pytest_evm-0.1.2/pytest_evm/fixtures.py
+-rw-r--r--   0        0        0     1956 2024-04-17 17:38:49.298623 pytest_evm-0.1.2/pytest_evm/hooks.py
+-rw-r--r--   0        0        0       62 2023-12-04 17:21:05.182141 pytest_evm-0.1.2/pytest_evm/pytest.ini
+-rw-r--r--   0        0        0     2040 2024-04-20 10:07:28.231512 pytest_evm-0.1.2/pytest_evm/utils.py
+-rw-r--r--   0        0        0     5511 1970-01-01 00:00:00.000000 pytest_evm-0.1.2/PKG-INFO
```

### Comparing `pytest_evm-0.1.1/LICENSE` & `pytest_evm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_evm-0.1.1/README.md` & `pytest_evm-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -101,16 +101,17 @@
 @pytest.fixture(scope="session")
 def eth_amount():
     amount = AsyncWeb3.to_wei(0.001, 'ether')
     return amount
 ```
 
 ## Test Reporting
-If your test performs one transaction, you can automatically `assert` transaction status and get useful report after test,
-if it completed successfully. To do this, you need to add mark `pytest.mark.tx` to your test.
+If your want to test one transaction, you can automatically `assert` transaction status and get useful report after test,
+if it completed successfully. To do this, you need to add mark `pytest.mark.tx` to your test and you must **return 
+transaction hash in test**
 
 ```python
 import pytest
 
 @pytest.mark.tx
 @pytest.mark.asyncio
 async def test_transaction(wallet, eth_amount):
@@ -124,14 +125,15 @@
 ![Test Report](https://i.ibb.co/n8vKXwB/Screenshot-2024-01-24-at-22-08-29.png)
          
 ## Usage Example
 Here is example of testing with `pytest-evm`:
 
 ```python
 import pytest
+from bridge import Bridge
 
 class TestBridge:
     @pytest.mark.tx
     @pytest.mark.asyncio
     async def test_swap(self, wallet, eth_amount, bridge, destination_network):
         return await bridge.swap(eth_amount, destination_network)
```

### Comparing `pytest_evm-0.1.1/pyproject.toml` & `pytest_evm-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'pytest_evm'
-version = '0.1.1'
+version = '0.1.2'
 description = 'The testing package containing tools to test Web3-based projects'
 authors = ['Alexey <abelenkov2006@gmail.com>']
 license = 'MIT'
 readme = 'README.md'
 repository = 'https://github.com/blnkoff/pytest-evm'
 homepage = 'https://github.com/blnkoff/pytest-evm'
 classifiers = [
```

### Comparing `pytest_evm-0.1.1/pytest_evm/fixtures.py` & `pytest_evm-0.1.2/pytest_evm/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_evm-0.1.1/pytest_evm/hooks.py` & `pytest_evm-0.1.2/pytest_evm/hooks.py`

 * *Files identical despite different names*

### Comparing `pytest_evm-0.1.1/pytest_evm/utils.py` & `pytest_evm-0.1.2/pytest_evm/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import time
 from functools import wraps
 from evm_wallet import Wallet
 from hexbytes import HexBytes
 from web3 import Web3
 from web3.middleware import geth_poa_middleware
+from pytest_evm.exceptions import TransactionStatusError
 
 
 def validate_status(func):
     @wraps(func)
     async def wrapper(*args, **kwargs):
-        wallet = kwargs['wallet']
+        wallet: Wallet = kwargs['wallet']
         tx_hash = await func(*args, **kwargs)
         status = (await wallet.provider.eth.wait_for_transaction_receipt(tx_hash)).get('status')
-        assert status
+        if not status:
+            explorer_url = wallet.get_explorer_url(tx_hash)
+            raise TransactionStatusError(explorer_url)
 
     return wrapper
 
 
 def get_last_transaction(wallet: Wallet, timeout: float = 10):
     w3 = Web3(Web3.HTTPProvider(wallet.network['rpc']))
     w3.middleware_onion.inject(geth_poa_middleware, layer=0)
```

### Comparing `pytest_evm-0.1.1/PKG-INFO` & `pytest_evm-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_evm
-Version: 0.1.1
+Version: 0.1.2
 Summary: The testing package containing tools to test Web3-based projects
 Home-page: https://github.com/blnkoff/pytest-evm
 License: MIT
 Author: Alexey
 Author-email: abelenkov2006@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -131,16 +131,17 @@
 @pytest.fixture(scope="session")
 def eth_amount():
     amount = AsyncWeb3.to_wei(0.001, 'ether')
     return amount
 ```
 
 ## Test Reporting
-If your test performs one transaction, you can automatically `assert` transaction status and get useful report after test,
-if it completed successfully. To do this, you need to add mark `pytest.mark.tx` to your test.
+If your want to test one transaction, you can automatically `assert` transaction status and get useful report after test,
+if it completed successfully. To do this, you need to add mark `pytest.mark.tx` to your test and you must **return 
+transaction hash in test**
 
 ```python
 import pytest
 
 @pytest.mark.tx
 @pytest.mark.asyncio
 async def test_transaction(wallet, eth_amount):
@@ -154,14 +155,15 @@
 ![Test Report](https://i.ibb.co/n8vKXwB/Screenshot-2024-01-24-at-22-08-29.png)
          
 ## Usage Example
 Here is example of testing with `pytest-evm`:
 
 ```python
 import pytest
+from bridge import Bridge
 
 class TestBridge:
     @pytest.mark.tx
     @pytest.mark.asyncio
     async def test_swap(self, wallet, eth_amount, bridge, destination_network):
         return await bridge.swap(eth_amount, destination_network)
```

