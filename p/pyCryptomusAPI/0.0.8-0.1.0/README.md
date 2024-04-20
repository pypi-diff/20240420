# Comparing `tmp/pyCryptomusAPI-0.0.8.tar.gz` & `tmp/pyCryptomusAPI-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCryptomusAPI-0.0.8.tar", last modified: Mon Aug 21 10:07:33 2023, max compression
+gzip compressed data, was "pyCryptomusAPI-0.1.0.tar", last modified: Sat Apr 20 19:15:34 2024, max compression
```

## Comparing `pyCryptomusAPI-0.0.8.tar` & `pyCryptomusAPI-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-21 10:07:33.467147 pyCryptomusAPI-0.0.8/
--rw-rw-rw-   0        0        0     1085 2022-12-10 18:10:42.000000 pyCryptomusAPI-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       40 2023-08-06 20:01:08.000000 pyCryptomusAPI-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2174 2023-08-21 10:07:33.467147 pyCryptomusAPI-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1672 2022-12-12 17:35:04.000000 pyCryptomusAPI-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-21 10:07:33.451529 pyCryptomusAPI-0.0.8/pyCryptomusAPI/
--rw-rw-rw-   0        0        0       20 2022-12-10 22:13:53.000000 pyCryptomusAPI-0.0.8/pyCryptomusAPI/__init__.py
--rw-rw-rw-   0        0        0    24034 2023-08-21 09:55:35.000000 pyCryptomusAPI-0.0.8/pyCryptomusAPI/api.py
--rw-rw-rw-   0        0        0    10494 2023-08-21 09:50:51.000000 pyCryptomusAPI-0.0.8/pyCryptomusAPI/cryto_types.py
--rw-rw-rw-   0        0        0     2154 2023-08-21 09:52:47.000000 pyCryptomusAPI-0.0.8/pyCryptomusAPI/tests.py
--rw-rw-rw-   0        0        0       95 2023-08-21 08:50:13.000000 pyCryptomusAPI-0.0.8/pyCryptomusAPI/version.py
-drwxrwxrwx   0        0        0        0 2023-08-21 10:07:33.467147 pyCryptomusAPI-0.0.8/pyCryptomusAPI.egg-info/
--rw-rw-rw-   0        0        0     2174 2023-08-21 10:07:33.000000 pyCryptomusAPI-0.0.8/pyCryptomusAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-08-21 10:07:33.000000 pyCryptomusAPI-0.0.8/pyCryptomusAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-21 10:07:33.000000 pyCryptomusAPI-0.0.8/pyCryptomusAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-08-21 10:07:33.000000 pyCryptomusAPI-0.0.8/pyCryptomusAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-21 10:07:33.467147 pyCryptomusAPI-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-08-07 16:33:36.000000 pyCryptomusAPI-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 19:15:34.841377 pyCryptomusAPI-0.1.0/
+-rw-rw-rw-   0        0        0     1085 2022-12-10 18:10:42.000000 pyCryptomusAPI-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       40 2023-08-06 20:01:08.000000 pyCryptomusAPI-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2174 2024-04-20 19:15:34.841377 pyCryptomusAPI-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1672 2022-12-12 17:35:04.000000 pyCryptomusAPI-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 19:15:34.841377 pyCryptomusAPI-0.1.0/pyCryptomusAPI/
+-rw-rw-rw-   0        0        0       20 2022-12-10 22:13:53.000000 pyCryptomusAPI-0.1.0/pyCryptomusAPI/__init__.py
+-rw-rw-rw-   0        0        0    31737 2024-04-19 22:30:43.000000 pyCryptomusAPI-0.1.0/pyCryptomusAPI/api.py
+-rw-rw-rw-   0        0        0    12016 2024-04-19 22:31:51.000000 pyCryptomusAPI-0.1.0/pyCryptomusAPI/cryto_types.py
+-rw-rw-rw-   0        0        0     2206 2024-04-19 22:37:08.000000 pyCryptomusAPI-0.1.0/pyCryptomusAPI/tests.py
+-rw-rw-rw-   0        0        0       95 2024-04-19 22:35:30.000000 pyCryptomusAPI-0.1.0/pyCryptomusAPI/version.py
+drwxrwxrwx   0        0        0        0 2024-04-20 19:15:34.841377 pyCryptomusAPI-0.1.0/pyCryptomusAPI.egg-info/
+-rw-rw-rw-   0        0        0     2174 2024-04-20 19:15:34.000000 pyCryptomusAPI-0.1.0/pyCryptomusAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-04-20 19:15:34.000000 pyCryptomusAPI-0.1.0/pyCryptomusAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 19:15:34.000000 pyCryptomusAPI-0.1.0/pyCryptomusAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-20 19:15:34.000000 pyCryptomusAPI-0.1.0/pyCryptomusAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 19:15:34.856994 pyCryptomusAPI-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-08-07 16:33:36.000000 pyCryptomusAPI-0.1.0/setup.py
```

### Comparing `pyCryptomusAPI-0.0.8/LICENSE` & `pyCryptomusAPI-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.8/PKG-INFO` & `pyCryptomusAPI-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCryptomusAPI
-Version: 0.0.8
+Version: 0.1.0
 Summary: Python implementation of Cryptomus (https://cryptomus.com) pubilc API
 Home-page: https://github.com/Badiboy/pyCryptomusAPI
 Author: Badiboy
 License: MIT license
 Keywords: Crypto Pay API Cryptomus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyCryptomusAPI-0.0.8/README.md` & `pyCryptomusAPI-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.8/pyCryptomusAPI/api.py` & `pyCryptomusAPI-0.1.0/pyCryptomusAPI/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         """
         self.merchant_uuid = merchant_uuid
         self.payment_api_key = payment_api_key
         self.payout_api_key = payout_api_key
         self.print_errors = print_errors
         self.timeout = timeout
         self.add_request_params = add_request_params
-        if not(self.payment_api_key) and not(self.payout_api_key):
+        if (not self.payment_api_key) and (not self.payout_api_key):
             raise Exception("You must specify at least one API key.")
 
     def __request(self, method_url, mode, **kwargs):
         """
         Send request to API
 
         :param method_url: (String) API method url (part)
@@ -59,19 +59,19 @@
 
         if self.add_request_params:
             data.update(self.add_request_params)
 
         base_resp = None
         try:
             key = self.payment_api_key if (mode == 1) else self.payout_api_key
-            if not(key):
+            if not key:
                 raise pyCryptomusAPIException(-6, "Key is empty")
             if not(key.isascii()):
                 raise pyCryptomusAPIException(-6, "Key contains non-ascii characters")
-            if not(self.merchant_uuid):
+            if not self.merchant_uuid:
                 raise pyCryptomusAPIException(-6, "Merchant UUID is empty")
             if not(self.merchant_uuid.isascii()):
                 raise pyCryptomusAPIException(-6, "Merchant UUID contains non-ascii characters")
             json_dumps = json.dumps(data)
             # json_dumps = json.dumps(data, ensure_ascii=False, separators=(',', ':'))
             pre_sign = json_dumps if data else ""
             if pre_sign and not(pre_sign.isascii()):
@@ -240,15 +240,15 @@
         is_force_refund: (Bool, Optional) Refund all incoming payments to sender’s address
 
         * You need to pass one of the required parameters, if you pass both, the account will be identified by order_id
         """
         method = "wallet/block-address"
         params = {
         }
-        if not(wallet_uuid) and not(order_id):
+        if (not wallet_uuid) and (not order_id):
             raise pyCryptomusAPIException(0, "You need to pass one of the required parameters")
         if wallet_uuid:
             params["uuid"] = wallet_uuid
         if order_id:
             params["order_id"] = order_id
         if is_force_refund is not None:
             params["is_force_refund"] = is_force_refund
@@ -269,15 +269,15 @@
 
         * To refund payments you need to pass either uuid or order_id, if you pass both, the static wallet will be identified by uuid
         """
         method = "wallet/blocked-address-refund"
         params = {
             "address": address,
         }
-        if not(wallet_uuid) and not(order_id):
+        if (not wallet_uuid) and (not order_id):
             raise pyCryptomusAPIException(0, "You need to pass one of the required parameters")
         if wallet_uuid:
             params["uuid"] = wallet_uuid
         if order_id:
             params["order_id"] = order_id
         resp = self.__request(method, 1, **params).get("result")
         return resp
@@ -294,15 +294,15 @@
         order_id: (String[1..128], Optional if wallet_uuid set) Invoice order ID
 
         * To get the invoice status you need to pass one of the required parameters, if you pass both, the account will be identified by order_id
         """
         method = "payment/info"
         params = {
         }
-        if not(invoice_uuid) and not(order_id):
+        if (not invoice_uuid) and (not order_id):
             raise pyCryptomusAPIException(0, "You need to pass one of the required parameters")
         if invoice_uuid:
             params["uuid"] = invoice_uuid
         if order_id:
             params["order_id"] = order_id
         resp = self.__request(method, 1, **params).get("result")
         return Invoice.de_json(resp)
@@ -323,15 +323,15 @@
         * Invoice is identified by order_id or uuid, if you pass both, the account will be identified by uuid
         """
         method = "payment/refund"
         params = {
             "address": address,
             "is_subtract": is_subtract,
         }
-        if not(invoice_uuid) and not(order_id):
+        if (not invoice_uuid) and (not order_id):
             raise pyCryptomusAPIException(0, "You need to pass one of the required parameters")
         if invoice_uuid:
             params["uuid"] = invoice_uuid
         if order_id:
             params["order_id"] = order_id
         resp = self.__request(method, 1, **params).get("result")
         return Invoice.de_json(resp)
@@ -436,14 +436,177 @@
         https://doc.cryptomus.com/payments/list-of-services
         Requires PAYMENT API key
         """
         method = "payment/services"
         resp = self.__request(method, 1).get("result")
         return [Service.de_json(i) for i in resp]
 
+    """
+    Request
+    Query parameters
+    NAME	PARAMETER TYPE	DEFAULT VALUE	DEFINITION
+    amount*	string		Payout amount
+    currency*	string		
+    Currency code for the payout
+    If Currency if fiat, the to_currency parameter is required.
+    order_id*	
+    string
+    min:1
+    max:100
+    alpha_dash
+    Order ID in your system
+    The parameter should be a string consisting of alphabetic characters, numbers, underscores, and dashes. It should not contain any spaces or special characters.
+    The order_id must be unique within the merchant payouts
+    When we find an existing payout with order_id, we return its details, a new payout will not be created.
+    address*	string		The address of the wallet to which the withdrawal will be made
+    is_subtract*	boolean		
+    Defines where the withdrawal fee will be deducted
+    true - from your balance
+    false - from payout amount, the payout amount will be decreased
+    network*	string		
+    Blockchain network code
+    Not required when the currency/to_currency is a cryptocurrency and has only one network, for example BTC
+    url_callback			URL to which webhooks with payout status will be sent
+    to_currency			Cryptocurrency code in which the payout will be made. It is used when the currency parameter is fiat. See examples below
+    course_source	string
+    Available values
+    -
+    Binance
+    -
+    BinanceP2p
+    -
+    Exmo
+    -
+    Kucoin
+    -
+    Garantexio
+    Value from merchant's settings	
+    The service from which the exchange rates are taken for conversion in the invoice.
+    The parameter is applied only if the currency is fiat, otherwise the default value is taken from the merchant's settings.
+    from_currency	string	null	Allows to automatically convert the withdrawal amount and use the from_currency balance. Only USDT is available.
+    priority	
+    string
+    min: 4
+    max: 11
+    Available values
+    -
+    recommended
+    -
+    economy
+    -
+    high
+    -
+    highest
+    recommended	
+    The parameter for selecting the withdrawal priority. The cost of the withdrawal fee depends on the selected parameter.
+    This parameter is applied only in case of using the BTC, ETH, POLYGON, and BSC networks.
+    memo	
+    string
+    min: 1
+    max: 30
+    Additional identifier for TON, used to specify a particular recipient or target
+    * - mandatory parameter
+    """
+
+    def create_payout(self,
+              amount, currency, order_id, address, is_subtract, network,
+              url_callback = None, to_currency = None, course_source = None,
+              from_currency = None, priority = None, memo = None):
+        """
+        Creating a payout
+        https://doc.cryptomus.com/payouts/creating-payout
+        Requires PAYOUT API key
+
+        amount: (String) Payout amount
+        currency: (String) Currency code for the payout. If Currency if fiat, the to_currency parameter is required.
+        order_id: (String[1..100]) Order ID in your system. The parameter should be a string consisting of alphabetic characters, numbers, underscores, and dashes. It should not contain any spaces or special characters. The order_id must be unique within the merchant payouts. When we find an existing payout with order_id, we return its details, a new payout will not be created.
+        address: (String) The address of the wallet to which the withdrawal will be made
+        is_subtract: (Bool) Defines where the withdrawal fee will be deducted. true - from your balance. false - from payout amount, the payout amount will be decreased.
+        network: (String) Blockchain network code.Not required when the currency/to_currency is a cryptocurrency and has only one network, for example BTC
+        url_callback: (String, Optional) URL to which webhooks with payout status will be sent
+        to_currency: (String, Optional) Cryptocurrency code in which the payout will be made. It is used when the currency parameter is fiat.
+        course_source: (String, Optional) The service from which the exchange rates are taken for conversion in the invoice. The parameter is applied only if the currency is fiat, otherwise the default value is taken from the merchant's settings.
+        from_currency: (String, Optional) Allows to automatically convert the withdrawal amount and use the from_currency balance. Only USDT is available.
+        priority: (String, Optional) The parameter for selecting the withdrawal priority. The cost of the withdrawal fee depends on the selected parameter. This parameter is applied only in case of using the BTC, ETH, POLYGON, and BSC networks. Available values: recommended, economy, high, highest
+        memo: (String, Optional) Additional identifier for TON, used to specify a particular recipient or target
+        """
+        method = "payout"
+        params = {
+            "amount": str(amount),
+            "currency": currency,
+            "order_id": str(order_id),
+            "address": address,
+            "is_subtract": is_subtract,
+            "network": network,
+        }
+        if url_callback:
+            params["url_callback"] = url_callback
+        if to_currency:
+            params["to_currency"] = to_currency
+        if course_source:
+            params["course_source"] = course_source
+        if from_currency:
+            params["from_currency"] = from_currency
+        if priority:
+            params["priority"] = priority
+        if memo:
+            params["memo"] = memo
+        resp = self.__request(method, 2, **params).get("result")
+        return Payout.de_json(resp)
+
+    def payout_information(self,
+           payout_uuid = None, order_id = None):
+        """
+        Payout information
+        https://doc.cryptomus.com/payouts/payout-information
+        You need to pass one of the required parameters, if you pass both, the account will be identified by order_id
+        Requires PAYOUT API key
+
+        payout_uuid: (String, Optional if order_id set) Payout UUID
+        order_id: (String[1..128], Optional if wallet_uuid set) Payout order ID
+
+        * To get the payout information you need to pass one of the parameters, if you pass both, the payout will be identified by order_id
+        """
+        method = "payout/info"
+        params = {
+        }
+        if (not payout_uuid) and (not order_id):
+            raise pyCryptomusAPIException(0, "You need to pass one of the required parameters")
+        if payout_uuid:
+            params["uuid"] = payout_uuid
+        if order_id:
+            params["order_id"] = order_id
+        resp = self.__request(method, 1, **params).get("result")
+        return Payout.de_json(resp)
+
+    def payout_history(self, date_from = None, date_to = None, cursor = None):
+        """
+        Payout history
+        https://doc.cryptomus.com/payments/payment-history
+        Requires PAYOUT API key
+
+        date_from: (String, Optional) Filtering by creation date, from
+        date_to: (String, Optional) Filtering by creation date, to
+        cursor: (String, Optional) Page cursor (hash)
+        """
+        params = {
+        }
+        if date_from:
+            params["date_from"] = date_from.strftime(CryptomusDateFormat)
+        if date_to:
+            params["date_to"] = date_to.strftime(CryptomusDateFormat)
+        if cursor:
+            params["cursor"] = cursor
+        method = "payment/list"
+        if params:
+            resp = self.__request(method, 1, **params).get("result")
+        else:
+            resp = self.__request(method, 1).get("result")
+        return PayoutHistory.de_json(resp)
+
     def payout_services(self):
         """
         Get collection of all available payout services
         https://doc.cryptomus.com/payouts/list-of-services
         Requires PAYMOUT API key
         """
         method = "payout/services"
```

### Comparing `pyCryptomusAPI-0.0.8/pyCryptomusAPI/cryto_types.py` & `pyCryptomusAPI-0.1.0/pyCryptomusAPI/cryto_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import datetime
 import json
 from abc import ABC
 
 CryptomusDateFormat = "%Y-%m-%d %H:%M:%S"
 
 class Dictionaryable(ABC):
     """
@@ -126,17 +125,19 @@
         data = cls.check_json(json_dict)
         instance = super(Balance, cls).de_json(data, process_mode=1)
         data = data.get("balance")
         if not data:
             raise ValueError("Not a balance")
         if "merchant" in data:
             for item in data["merchant"]:
+                # noinspection PyUnresolvedReferences
                 instance.merchant.append(BalanceItem.de_json(item))
         if "user" in data:
             for item in data["user"]:
+                # noinspection PyUnresolvedReferences
                 instance.user.append(BalanceItem.de_json(item))
         return instance
 
 
 # noinspection PyMethodOverriding
 class ServiceLimit(JsonDeserializable):
     def __init__(self):
@@ -300,7 +301,48 @@
     @classmethod
     def de_json(cls, json_dict):
         data = cls.check_json(json_dict)
         instance = super(PaymentsHistory, cls).de_json(data, process_mode=2)
         instance.items = [Invoice.de_json(i) for i in instance.items]
         instance.paginate = PaymentPaginate.de_json(instance.paginate)
         return instance
+
+# noinspection PyMethodOverriding
+class Payout(JsonDeserializable):
+    def __init__(self):
+        self.uuid = None
+        self.amount = None
+        self.currency = None
+        self.network = None
+        self.address = None
+        self.txid = None
+        self.status = None
+        self.is_final = None
+        self.balance = None
+        self.payer_currency = None
+        self.payer_amount = None
+
+    @classmethod
+    def de_json(cls, json_dict):
+        data = cls.check_json(json_dict)
+        instance = super(Payout, cls).de_json(data, process_mode=2)
+        if instance.amount is not None:
+            instance.amount = float(instance.amount)
+        if instance.payer_amount is not None:
+            instance.payer_amount = float(instance.payer_amount)
+        if instance.balance is not None:
+            instance.balance = float(instance.balance)
+        return instance
+
+# noinspection PyMethodOverriding
+class PayoutHistory(JsonDeserializable):
+    def __init__(self):
+        self.items = []
+        self.paginate = PaymentPaginate()
+
+    @classmethod
+    def de_json(cls, json_dict):
+        data = cls.check_json(json_dict)
+        instance = super(PayoutHistory, cls).de_json(data, process_mode=2)
+        instance.items = [Payout.de_json(i) for i in instance.items]
+        instance.paginate = PaymentPaginate.de_json(instance.paginate)
+        return instance
```

### Comparing `pyCryptomusAPI-0.0.8/pyCryptomusAPI/tests.py` & `pyCryptomusAPI-0.1.0/pyCryptomusAPI/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,10 +46,11 @@
     run_and_print(lambda: client.block_wallet_refund(wallet_adress, wallet_uuid = wallet_uuid))  # Server error (it's ok)
     run_and_print(lambda: client.payment_information(invoice_uuid = invoice_uuid))
     run_and_print(lambda: client.refund(wallet_adress, True, invoice_uuid = invoice_uuid))       # Server error (looks ok)
     run_and_print(lambda: client.payment_services())
     run_and_print(lambda: client.payment_history())
     run_and_print(lambda: client.payment_history_filtered(is_final=True))
     run_and_print(lambda: client.payout_services())
+    run_and_print(lambda: client.payout_history())
     run_and_print(lambda: client.balance())
 
 test_api_functions()
```

### Comparing `pyCryptomusAPI-0.0.8/pyCryptomusAPI.egg-info/PKG-INFO` & `pyCryptomusAPI-0.1.0/pyCryptomusAPI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCryptomusAPI
-Version: 0.0.8
+Version: 0.1.0
 Summary: Python implementation of Cryptomus (https://cryptomus.com) pubilc API
 Home-page: https://github.com/Badiboy/pyCryptomusAPI
 Author: Badiboy
 License: MIT license
 Keywords: Crypto Pay API Cryptomus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyCryptomusAPI-0.0.8/setup.py` & `pyCryptomusAPI-0.1.0/setup.py`

 * *Files identical despite different names*

