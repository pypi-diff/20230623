# Comparing `tmp/breeze_strategies-6.0.8.tar.gz` & `tmp/breeze_strategies-6.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-6.0.8.tar", last modified: Fri Jun 23 07:15:21 2023, max compression
+gzip compressed data, was "breeze_strategies-6.0.9.tar", last modified: Fri Jun 23 07:53:51 2023, max compression
```

## Comparing `breeze_strategies-6.0.8.tar` & `breeze_strategies-6.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 07:15:21.634656 breeze_strategies-6.0.8/
--rw-rw-rw-   0        0        0     1113 2023-06-23 07:11:33.000000 breeze_strategies-6.0.8/LICENSE
--rw-rw-rw-   0        0        0     1292 2023-06-23 07:15:21.634656 breeze_strategies-6.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      741 2023-06-23 07:13:29.000000 breeze_strategies-6.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 07:15:21.567632 breeze_strategies-6.0.8/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.8/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    20102 2023-06-23 07:03:54.000000 breeze_strategies-6.0.8/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-23 07:15:21.634656 breeze_strategies-6.0.8/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1292 2023-06-23 07:15:21.000000 breeze_strategies-6.0.8/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-23 07:15:21.000000 breeze_strategies-6.0.8/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 07:15:21.000000 breeze_strategies-6.0.8/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-23 07:15:21.000000 breeze_strategies-6.0.8/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-23 07:15:21.000000 breeze_strategies-6.0.8/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 07:15:21.634656 breeze_strategies-6.0.8/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-06-23 07:12:57.000000 breeze_strategies-6.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:53:51.185161 breeze_strategies-6.0.9/
+-rw-rw-rw-   0        0        0     1113 2023-06-23 07:11:33.000000 breeze_strategies-6.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1292 2023-06-23 07:53:51.185161 breeze_strategies-6.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      741 2023-06-23 07:53:37.000000 breeze_strategies-6.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 07:53:51.117775 breeze_strategies-6.0.9/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.9/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    20174 2023-06-23 07:53:01.000000 breeze_strategies-6.0.9/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:53:51.177454 breeze_strategies-6.0.9/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1292 2023-06-23 07:53:50.000000 breeze_strategies-6.0.9/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-23 07:53:50.000000 breeze_strategies-6.0.9/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 07:53:50.000000 breeze_strategies-6.0.9/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-23 07:53:50.000000 breeze_strategies-6.0.9/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-23 07:53:50.000000 breeze_strategies-6.0.9/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 07:53:51.185161 breeze_strategies-6.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-06-23 07:53:45.000000 breeze_strategies-6.0.9/setup.py
```

### Comparing `breeze_strategies-6.0.8/LICENSE` & `breeze_strategies-6.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-6.0.8/PKG-INFO` & `breeze_strategies-6.0.9/breeze_strategies.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: breeze_strategies
-Version: 6.0.8
+Name: breeze-strategies
+Version: 6.0.9
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.8
+pip install breeze_strategies==6.0.9
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.8/README.md` & `breeze_strategies-6.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.8
+pip install breeze_strategies==6.0.9
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.8/breeze_strategies/breeze_strategies.py` & `breeze_strategies-6.0.9/breeze_strategies/breeze_strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,14 +188,15 @@
                     expiry_date = expiry_date,
                     right= right,
                     strike_price=strike_price)
             response = None
             if(data['Status'] == 200):
                 response = data['Success']['message']
                 print(f"Success : {response} for {right} with order_id :{data['Success']['order_id']}")
+                res_queue.put(data)
             else:
                 response = data['Error']
                 print(f"Error : {response} for {right}")
                 res_queue.put(data)
             return(data)
                   
         res_queue = queue.Queue()
@@ -321,15 +322,16 @@
                 print("Call order got executed at price :{0} Rs and Put Order got executed at price : {1} Rs".format(call_execution,put_execution))
                 self.profit_and_loss(product_type, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution)
             
     
     
     
     def stop(self):
-        self.client.ws_disconnect()
+        if(self.socket == 1):
+            self.client.ws_disconnect()
         self.socket = 0
         time.sleep(1)
         print("Squaring off the both contracts and exiting strategy...")
         print("----------------------------------------")
         
         square_call = self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Call")
         square_put = self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Put")
```

### Comparing `breeze_strategies-6.0.8/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-6.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: breeze-strategies
-Version: 6.0.8
+Name: breeze_strategies
+Version: 6.0.9
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.8
+pip install breeze_strategies==6.0.9
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.8/setup.py` & `breeze_strategies-6.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="6.0.8",
+    version="6.0.9",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

