# Comparing `tmp/phonepe-1.0.0.tar.gz` & `tmp/phonepe-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonepe-1.0.0.tar", last modified: Tue Jul 11 17:03:11 2023, max compression
+gzip compressed data, was "phonepe-1.0.1.tar", last modified: Wed Jul 12 16:32:50 2023, max compression
```

## Comparing `phonepe-1.0.0.tar` & `phonepe-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:03:11.293670 phonepe-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-11 17:03:11.293670 phonepe-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-11 17:02:57.000000 phonepe-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:03:11.293670 phonepe-1.0.0/phonepe/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:02:57.000000 phonepe-1.0.0/phonepe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-11 17:02:57.000000 phonepe-1.0.0/phonepe/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:03:11.293670 phonepe-1.0.0/phonepe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-11 17:03:11.000000 phonepe-1.0.0/phonepe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-11 17:03:11.000000 phonepe-1.0.0/phonepe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:03:11.000000 phonepe-1.0.0/phonepe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:03:11.000000 phonepe-1.0.0/phonepe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 17:03:11.000000 phonepe-1.0.0/phonepe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:03:11.293670 phonepe-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-11 17:02:57.000000 phonepe-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:50.732046 phonepe-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-12 16:32:50.732046 phonepe-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-12 16:32:39.000000 phonepe-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:50.728046 phonepe-1.0.1/phonepe/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 16:32:39.000000 phonepe-1.0.1/phonepe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-07-12 16:32:39.000000 phonepe-1.0.1/phonepe/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:50.732046 phonepe-1.0.1/phonepe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-12 16:32:50.000000 phonepe-1.0.1/phonepe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-12 16:32:50.000000 phonepe-1.0.1/phonepe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:32:50.000000 phonepe-1.0.1/phonepe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 16:32:50.000000 phonepe-1.0.1/phonepe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 16:32:50.000000 phonepe-1.0.1/phonepe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 16:32:50.732046 phonepe-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-12 16:32:39.000000 phonepe-1.0.1/setup.py
```

### Comparing `phonepe-1.0.0/PKG-INFO` & `phonepe-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonepe
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python library for interacting with PhonePe Payment Gateway API.
 Home-page: https://github.com/devbijay/phonepe-pg
 Author: Bijay Nayak
 Author-email: bijay6779@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -43,24 +43,23 @@
    phone_pe_salt (str): The PhonePe salt.
    redirect_url (str): The redirect URL.
    webhook_url (str): The webhook URL.
    phone_pe_salt_index (int, optional): The PhonePe salt index. Defaults to 1.
    redirect_mode (str, optional): The redirect mode. Defaults to "GET". Valid Values "GET/POST"
 ```
 
-* Create CheckSum And base64 encoded payment data
+* Create Transaction With Order Data
 ```python
-check_sum, encoded_order_payload = phonepe.create_order("ORDER_ID", 100, "USER_ID")
+order_data= phonepe.create_txn("ORDER_ID", 100, "USER_ID")
 
-#Create Transaction Link
-phonepe_txn = phonepe.create_phone_pe_txn(check_sum, encoded_order_payload)
+#Extract Payment Link
+link = order_data["data"]["instrumentResponse"]["redirectInfo"]["url"]
 
-print(phonepe_txn)
+print(link)
 ```
-* Note: Please Store The Checksum If You Are Updating The Transaction Status Via Webhook Callback
 * The payload that is going to be sent to the merchant on the specified callback URL will have a base64 encoded JSON.
 * Upon base64 decoding the response, you should get a JSON with a format similar to the response returned by transaction status API.
 Following are the response headers sent with a callback.
 
 * Please follow [this documentation](http://developer.phonepe.com/v1/reference/server-to-server-callback-5) if you are updating the paymenty status via  
 webhook
 
@@ -85,15 +84,14 @@
         "url": "https://mercury-uat.phonepe.com/transact/pg?token=NGVjMzhjOWMzMGI5ODI2OWMwYmQ2MzUzYWE2ZDYzZGM0M2M0NjZkNjVjMWRmNzlmODk1YWEwNjViMTUwNjYyOTI4NDY1OWExYzNmMjQzNjYzZjgxOTQzYjVjMGUyMmYyZGZhMTg5ODRlZDM2MzEzNWYyZDViOTdkZmU2NjFjOGU3ZTdiMzNlNzpmM2ZkZDYwY2JmNGFiYTUxM2Y3OGJhNGVjOTQ5OWU1NQ",
         "method": "GET"
       }
     }
   }
 }
 ```
-You can use the `phonepe_txn['data']['instrumentResponse']['redirectInfo']['url']` to access the hosted checkout link
 ### Check Transaction Status
 
 The following code shows how to check the status of a PhonePe transaction:
 
 ```python
 
 status = phonepe.check_txn_status("MERCHANT_TXN_ID")
@@ -122,14 +120,18 @@
 ```
 
 * S2S and Check Status API Handling
 
 Once the customer is redirected back to the merchant website/app, merchants should check with their server if they have received the Server-to-Server Callback response. If not, it is mandatory to make a Transaction Status API check with PhonePe backend systems to know the actual status of the payment and, then accordingly process the result.
 
 The payment status can be Success, Failed or Pending. When Pending, merchants should retry until the status changes to Success or Failed.
+```python
+if phonepe.verify_webhook_checksum(check_sum_in_header:str, b64_encoded_order_data:dict):
+    update_payment_status_in_db()
+```
 
 ```html
 Check Status API - Reconciliation [MANDATORY]
 
 If the payment status is Pending, then Check Status API should be called in the following interval:
 The first status check at 20-25 seconds post transaction start, then
 Every 3 seconds once for the next 30 seconds,
@@ -182,26 +184,24 @@
     phone_pe_salt="099eb0cd-02cf-4e2a-8aca-3e6c6aff0399",
     phone_pe_host="https://api-preprod.phonepe.com/apis/pg-sandbox",
     redirect_url="https://webhook.site/42fb84f2-1831-4467-9199-6bf0b839dc69",
     webhook_url="https://webhook.site/42fb84f2-1831-4467-9199-6bf0b839dc69"
 )
 
 # Create PhonePe Order
-checksum, txn_data = phonepe.create_order("OTGTRT156", 1000, "bijay")
-resp = phonepe.create_phone_pe_txn(checksum, txn_data)
-payment_link = resp["data"]["instrumentResponse"]["redirectInfo"]["url"]
+order_data = phonepe.create_txn("OTGTRT156", 1000, "bijay")
+payment_link = order_data["data"]["instrumentResponse"]["redirectInfo"]["url"]
 
 # Check Transaction Status
 txn_status = phonepe.check_txn_status(resp['data']['merchantTransactionId'])
 
 # Refund PhonePe Order
 refund = RefundTxn(txn_user_id="bijay", merchant_order_id="OTGTRT156", phonepe_txn_id="T2307112141199670477007",
                    amount=1000)
 ref_resp = phonepe.refund_txn(refund)
-
 ```
 
 For more information, please see the official [documentation](https://developer.phonepe.com/v1/reference/pay-api-1).
 
 
 I hope this is helpful! Let me know if you have any other questions.
 ```
```

### Comparing `phonepe-1.0.0/README.md` & `phonepe-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,24 +27,23 @@
    phone_pe_salt (str): The PhonePe salt.
    redirect_url (str): The redirect URL.
    webhook_url (str): The webhook URL.
    phone_pe_salt_index (int, optional): The PhonePe salt index. Defaults to 1.
    redirect_mode (str, optional): The redirect mode. Defaults to "GET". Valid Values "GET/POST"
 ```
 
-* Create CheckSum And base64 encoded payment data
+* Create Transaction With Order Data
 ```python
-check_sum, encoded_order_payload = phonepe.create_order("ORDER_ID", 100, "USER_ID")
+order_data= phonepe.create_txn("ORDER_ID", 100, "USER_ID")
 
-#Create Transaction Link
-phonepe_txn = phonepe.create_phone_pe_txn(check_sum, encoded_order_payload)
+#Extract Payment Link
+link = order_data["data"]["instrumentResponse"]["redirectInfo"]["url"]
 
-print(phonepe_txn)
+print(link)
 ```
-* Note: Please Store The Checksum If You Are Updating The Transaction Status Via Webhook Callback
 * The payload that is going to be sent to the merchant on the specified callback URL will have a base64 encoded JSON.
 * Upon base64 decoding the response, you should get a JSON with a format similar to the response returned by transaction status API.
 Following are the response headers sent with a callback.
 
 * Please follow [this documentation](http://developer.phonepe.com/v1/reference/server-to-server-callback-5) if you are updating the paymenty status via  
 webhook
 
@@ -69,15 +68,14 @@
         "url": "https://mercury-uat.phonepe.com/transact/pg?token=NGVjMzhjOWMzMGI5ODI2OWMwYmQ2MzUzYWE2ZDYzZGM0M2M0NjZkNjVjMWRmNzlmODk1YWEwNjViMTUwNjYyOTI4NDY1OWExYzNmMjQzNjYzZjgxOTQzYjVjMGUyMmYyZGZhMTg5ODRlZDM2MzEzNWYyZDViOTdkZmU2NjFjOGU3ZTdiMzNlNzpmM2ZkZDYwY2JmNGFiYTUxM2Y3OGJhNGVjOTQ5OWU1NQ",
         "method": "GET"
       }
     }
   }
 }
 ```
-You can use the `phonepe_txn['data']['instrumentResponse']['redirectInfo']['url']` to access the hosted checkout link
 ### Check Transaction Status
 
 The following code shows how to check the status of a PhonePe transaction:
 
 ```python
 
 status = phonepe.check_txn_status("MERCHANT_TXN_ID")
@@ -106,14 +104,18 @@
 ```
 
 * S2S and Check Status API Handling
 
 Once the customer is redirected back to the merchant website/app, merchants should check with their server if they have received the Server-to-Server Callback response. If not, it is mandatory to make a Transaction Status API check with PhonePe backend systems to know the actual status of the payment and, then accordingly process the result.
 
 The payment status can be Success, Failed or Pending. When Pending, merchants should retry until the status changes to Success or Failed.
+```python
+if phonepe.verify_webhook_checksum(check_sum_in_header:str, b64_encoded_order_data:dict):
+    update_payment_status_in_db()
+```
 
 ```html
 Check Status API - Reconciliation [MANDATORY]
 
 If the payment status is Pending, then Check Status API should be called in the following interval:
 The first status check at 20-25 seconds post transaction start, then
 Every 3 seconds once for the next 30 seconds,
@@ -166,26 +168,24 @@
     phone_pe_salt="099eb0cd-02cf-4e2a-8aca-3e6c6aff0399",
     phone_pe_host="https://api-preprod.phonepe.com/apis/pg-sandbox",
     redirect_url="https://webhook.site/42fb84f2-1831-4467-9199-6bf0b839dc69",
     webhook_url="https://webhook.site/42fb84f2-1831-4467-9199-6bf0b839dc69"
 )
 
 # Create PhonePe Order
-checksum, txn_data = phonepe.create_order("OTGTRT156", 1000, "bijay")
-resp = phonepe.create_phone_pe_txn(checksum, txn_data)
-payment_link = resp["data"]["instrumentResponse"]["redirectInfo"]["url"]
+order_data = phonepe.create_txn("OTGTRT156", 1000, "bijay")
+payment_link = order_data["data"]["instrumentResponse"]["redirectInfo"]["url"]
 
 # Check Transaction Status
 txn_status = phonepe.check_txn_status(resp['data']['merchantTransactionId'])
 
 # Refund PhonePe Order
 refund = RefundTxn(txn_user_id="bijay", merchant_order_id="OTGTRT156", phonepe_txn_id="T2307112141199670477007",
                    amount=1000)
 ref_resp = phonepe.refund_txn(refund)
-
 ```
 
 For more information, please see the official [documentation](https://developer.phonepe.com/v1/reference/pay-api-1).
 
 
 I hope this is helpful! Let me know if you have any other questions.
 ```
```

### Comparing `phonepe-1.0.0/phonepe/main.py` & `phonepe-1.0.1/phonepe/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -102,14 +102,31 @@
         }
         try:
             response = requests.post(f"{self.phone_pe_host}/pg/v1/pay", json=payload, headers=headers)
             return response.json()
         except Exception:
             return None
 
+    def create_txn(self, order_id, amount, user):
+        """
+            Creates a PhonePe transaction.
+
+            This method generates a PhonePe transaction by creating an order, calculating the checksum, and invoking the PhonePe transaction creation API.
+
+            Args:
+                order_id (str): The unique ID for the order.
+                amount (float): The transaction amount.
+                user (str): The user associated with the transaction.
+
+            Returns:
+                Transaction Response: The created PhonePe transaction.
+    """
+        check_sum, order_data = self.create_order(order_id, amount, user)
+        return self.create_phone_pe_txn(check_sum, order_data)
+
     def check_txn_status(self, merchant_txn_id):
         """
             Checks the status of a PhonePe transaction.
 
             Args:
                 merchant_txn_id: The merchant transaction ID.
 
@@ -122,15 +139,14 @@
         headers = {
             "accept": "application/json",
             "Content-Type": "application/json",
             "X-VERIFY": sha_header,
             "X-MERCHANT-ID": self.merchant_id
         }
 
-
         print(headers)
         try:
             response = requests.get(base_url, headers=headers)
             return response.json()
         except Exception:
             return None
 
@@ -166,14 +182,31 @@
         url = f"{self.phone_pe_host}/pg/v1/refund"
         try:
             response = requests.post(url, json=payload, headers=headers)
             return response.json()
         except Exception:
             return None
 
+    def verify_webhook_checksum(self, check_sum: str, order_data: dict) -> bool:
+        """
+            Verifies the integrity of a webhook checksum with base64_encoded payment data.
+
+            This method is used to validate the checksum received in the response of a Server to Server callback with the checksum calculated at your end.
+
+            Args:
+                check_sum (str): The checksum received in the webhook response X-VERIFY header.
+                order_data (str): The response received in webhook payload.
+
+            Returns:
+                bool: True if the calculated checksum matches the received checksum, False otherwise.
+        """
+
+        return self.sha256_encode(order_data['response'] + self.phone_pe_salt) + '###' + str(
+            self.phone_pe_salt_index) == check_sum
+
     def verify_vpa(self, vpa_address):
         """
             Validates a PhonePe VPA address.
 
             Args:
                 vpa_address: The VPA address to validate.
```

### Comparing `phonepe-1.0.0/phonepe.egg-info/PKG-INFO` & `phonepe-1.0.1/phonepe.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonepe
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python library for interacting with PhonePe Payment Gateway API.
 Home-page: https://github.com/devbijay/phonepe-pg
 Author: Bijay Nayak
 Author-email: bijay6779@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -43,24 +43,23 @@
    phone_pe_salt (str): The PhonePe salt.
    redirect_url (str): The redirect URL.
    webhook_url (str): The webhook URL.
    phone_pe_salt_index (int, optional): The PhonePe salt index. Defaults to 1.
    redirect_mode (str, optional): The redirect mode. Defaults to "GET". Valid Values "GET/POST"
 ```
 
-* Create CheckSum And base64 encoded payment data
+* Create Transaction With Order Data
 ```python
-check_sum, encoded_order_payload = phonepe.create_order("ORDER_ID", 100, "USER_ID")
+order_data= phonepe.create_txn("ORDER_ID", 100, "USER_ID")
 
-#Create Transaction Link
-phonepe_txn = phonepe.create_phone_pe_txn(check_sum, encoded_order_payload)
+#Extract Payment Link
+link = order_data["data"]["instrumentResponse"]["redirectInfo"]["url"]
 
-print(phonepe_txn)
+print(link)
 ```
-* Note: Please Store The Checksum If You Are Updating The Transaction Status Via Webhook Callback
 * The payload that is going to be sent to the merchant on the specified callback URL will have a base64 encoded JSON.
 * Upon base64 decoding the response, you should get a JSON with a format similar to the response returned by transaction status API.
 Following are the response headers sent with a callback.
 
 * Please follow [this documentation](http://developer.phonepe.com/v1/reference/server-to-server-callback-5) if you are updating the paymenty status via  
 webhook
 
@@ -85,15 +84,14 @@
         "url": "https://mercury-uat.phonepe.com/transact/pg?token=NGVjMzhjOWMzMGI5ODI2OWMwYmQ2MzUzYWE2ZDYzZGM0M2M0NjZkNjVjMWRmNzlmODk1YWEwNjViMTUwNjYyOTI4NDY1OWExYzNmMjQzNjYzZjgxOTQzYjVjMGUyMmYyZGZhMTg5ODRlZDM2MzEzNWYyZDViOTdkZmU2NjFjOGU3ZTdiMzNlNzpmM2ZkZDYwY2JmNGFiYTUxM2Y3OGJhNGVjOTQ5OWU1NQ",
         "method": "GET"
       }
     }
   }
 }
 ```
-You can use the `phonepe_txn['data']['instrumentResponse']['redirectInfo']['url']` to access the hosted checkout link
 ### Check Transaction Status
 
 The following code shows how to check the status of a PhonePe transaction:
 
 ```python
 
 status = phonepe.check_txn_status("MERCHANT_TXN_ID")
@@ -122,14 +120,18 @@
 ```
 
 * S2S and Check Status API Handling
 
 Once the customer is redirected back to the merchant website/app, merchants should check with their server if they have received the Server-to-Server Callback response. If not, it is mandatory to make a Transaction Status API check with PhonePe backend systems to know the actual status of the payment and, then accordingly process the result.
 
 The payment status can be Success, Failed or Pending. When Pending, merchants should retry until the status changes to Success or Failed.
+```python
+if phonepe.verify_webhook_checksum(check_sum_in_header:str, b64_encoded_order_data:dict):
+    update_payment_status_in_db()
+```
 
 ```html
 Check Status API - Reconciliation [MANDATORY]
 
 If the payment status is Pending, then Check Status API should be called in the following interval:
 The first status check at 20-25 seconds post transaction start, then
 Every 3 seconds once for the next 30 seconds,
@@ -182,26 +184,24 @@
     phone_pe_salt="099eb0cd-02cf-4e2a-8aca-3e6c6aff0399",
     phone_pe_host="https://api-preprod.phonepe.com/apis/pg-sandbox",
     redirect_url="https://webhook.site/42fb84f2-1831-4467-9199-6bf0b839dc69",
     webhook_url="https://webhook.site/42fb84f2-1831-4467-9199-6bf0b839dc69"
 )
 
 # Create PhonePe Order
-checksum, txn_data = phonepe.create_order("OTGTRT156", 1000, "bijay")
-resp = phonepe.create_phone_pe_txn(checksum, txn_data)
-payment_link = resp["data"]["instrumentResponse"]["redirectInfo"]["url"]
+order_data = phonepe.create_txn("OTGTRT156", 1000, "bijay")
+payment_link = order_data["data"]["instrumentResponse"]["redirectInfo"]["url"]
 
 # Check Transaction Status
 txn_status = phonepe.check_txn_status(resp['data']['merchantTransactionId'])
 
 # Refund PhonePe Order
 refund = RefundTxn(txn_user_id="bijay", merchant_order_id="OTGTRT156", phonepe_txn_id="T2307112141199670477007",
                    amount=1000)
 ref_resp = phonepe.refund_txn(refund)
-
 ```
 
 For more information, please see the official [documentation](https://developer.phonepe.com/v1/reference/pay-api-1).
 
 
 I hope this is helpful! Let me know if you have any other questions.
 ```
```

### Comparing `phonepe-1.0.0/setup.py` & `phonepe-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'A Python library for interacting with PhonePe Payment Gateway API.'
 LONG_DESCRIPTION = 'This Python package provides a simple interface to the PhonePe Payment Gateway. It can be used to ' \
                    'create PhonePe payment links, check the status of PhonePe transactions, and refund PhonePe ' \
                    'transactions. '
 
 
 setup(
```

