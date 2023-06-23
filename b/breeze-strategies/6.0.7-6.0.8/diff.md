# Comparing `tmp/breeze_strategies-6.0.7.tar.gz` & `tmp/breeze_strategies-6.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-6.0.7.tar", last modified: Thu Jun 22 09:35:59 2023, max compression
+gzip compressed data, was "breeze_strategies-6.0.8.tar", last modified: Fri Jun 23 07:15:21 2023, max compression
```

## Comparing `breeze_strategies-6.0.7.tar` & `breeze_strategies-6.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 09:35:59.570940 breeze_strategies-6.0.7/
--rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-6.0.7/LICENSE
--rw-rw-rw-   0        0        0     1135 2023-06-22 09:35:59.569941 breeze_strategies-6.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-06-22 09:35:52.000000 breeze_strategies-6.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 09:35:59.536572 breeze_strategies-6.0.7/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.7/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    20618 2023-06-22 09:35:37.000000 breeze_strategies-6.0.7/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-22 09:35:59.567943 breeze_strategies-6.0.7/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1135 2023-06-22 09:35:59.000000 breeze_strategies-6.0.7/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-22 09:35:59.000000 breeze_strategies-6.0.7/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 09:35:59.000000 breeze_strategies-6.0.7/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-22 09:35:59.000000 breeze_strategies-6.0.7/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-22 09:35:59.000000 breeze_strategies-6.0.7/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 09:35:59.571940 breeze_strategies-6.0.7/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-06-22 09:35:45.000000 breeze_strategies-6.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:15:21.634656 breeze_strategies-6.0.8/
+-rw-rw-rw-   0        0        0     1113 2023-06-23 07:11:33.000000 breeze_strategies-6.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1292 2023-06-23 07:15:21.634656 breeze_strategies-6.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      741 2023-06-23 07:13:29.000000 breeze_strategies-6.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 07:15:21.567632 breeze_strategies-6.0.8/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.8/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    20102 2023-06-23 07:03:54.000000 breeze_strategies-6.0.8/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:15:21.634656 breeze_strategies-6.0.8/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1292 2023-06-23 07:15:21.000000 breeze_strategies-6.0.8/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-23 07:15:21.000000 breeze_strategies-6.0.8/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 07:15:21.000000 breeze_strategies-6.0.8/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-23 07:15:21.000000 breeze_strategies-6.0.8/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-23 07:15:21.000000 breeze_strategies-6.0.8/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 07:15:21.634656 breeze_strategies-6.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-06-23 07:12:57.000000 breeze_strategies-6.0.8/setup.py
```

### Comparing `breeze_strategies-6.0.7/LICENSE` & `breeze_strategies-6.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-6.0.7/PKG-INFO` & `breeze_strategies-6.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze_strategies
-Version: 6.0.7
+Version: 6.0.8
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,28 +17,31 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.7
+pip install breeze_strategies==6.0.8
 
 ```
 
 
 ## code usage
 
 ```python
 
 from breeze_strategies import Strategies
 
 
 obj = Strategies(app_key = "your app key",secret_key = "your secret key",api_session = "your api session",max_profit = "your max profit",max_loss = "your max loss")
-obj.long_straddle(stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
+obj.straddle(strategy_type = "long",stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
+
+obj.straddle(strategy_type = "short",stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
+
 obj.stop() #for disconnection and exit of current strategy
 obj.get_pnl()
 
 ```
```

### Comparing `breeze_strategies-6.0.7/README.md` & `breeze_strategies-6.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.7
+pip install breeze_strategies==6.0.8
 
 ```
 
 
 ## code usage
 
 ```python
 
 from breeze_strategies import Strategies
 
 
 obj = Strategies(app_key = "your app key",secret_key = "your secret key",api_session = "your api session",max_profit = "your max profit",max_loss = "your max loss")
-obj.long_straddle(stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
+obj.straddle(strategy_type = "long",stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
+
+obj.straddle(strategy_type = "short",stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
+
 obj.stop() #for disconnection and exit of current strategy
 obj.get_pnl()
 
 ```
```

### Comparing `breeze_strategies-6.0.7/breeze_strategies/breeze_strategies.py` & `breeze_strategies-6.0.8/breeze_strategies/breeze_strategies.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,29 +18,37 @@
         self.maxloss = int(max_loss)
         self.maxprofit = int(max_profit)
         self.currentcall = 0
         self.currentput = 0
         self.flag = False
         self.client = BreezeConnect(app_key)
         self.client.generate_session(secret_key,api_session)
-        self.client.ws_connect()
+        
         self.quantity = 0
         self.exchange_code = ""
         self.stock_code = ""
         self.product_type = ""
         self.expiry_date = ""
         self.strike_price = ""
         self.order_type = ""
         self.validity = ""
         self.stoploss = ""
         self.validity_date = ""
         self.callexecution = ""
         self.putexecution = ""
+        self.strategy_type = ""
+        self.socket = 0
     
-    def squareoff(self,exchange_code, stock_code, product_type, expiry_date, strike_price, action, order_type, validity, stoploss, quantity, price,validity_date, trade_password, disclosed_quantity,right):
+    def squareoff(self,exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, price,validity_date, trade_password, disclosed_quantity,right):
+        action = "buy"
+        if(self.strategy_type.lower() == "short"):
+            action = "buy"
+        else:
+            action = "sell"
+
         data = self.client.square_off(exchange_code=exchange_code,
                             product="options",
                             stock_code=stock_code,
                             expiry_date=expiry_date,
                             right=right,
                             strike_price=strike_price,
                             action=action,
@@ -83,118 +91,132 @@
         day = expiry_date[8:10]
         formatted_date = f"{day}-{month_names[month]}-{year}"
         return(formatted_date)
         
     def trigger(self,product_type, rightval, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution,put_execution):
         net_gain_loss = (self.currentcall + self.currentput)*int(quantity)
         print(f"P&L (NET) : {round(net_gain_loss,2)}/- Rs")
-        print("-------------------------------------------------------------------")
+        print("----------------------------------------")
         formatted_date = self.get_date_format(expiry_date)
 
         if(net_gain_loss > 0 and net_gain_loss >= self.maxprofit):
-            print("maxprofit has reached...")
-            print("SquareOff operation on both contracts call and put begins....")
+            print("TakeProfit reached...")
+            #print("SquareOff operation on both contracts call and put begins....")
             
-            #self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Call",action = "sell", price = "")
-            #self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price , order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Put", action = "sell", price = "")
             
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Call", get_exchange_quotes=True, get_market_depth=False)
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Put", get_exchange_quotes=True, get_market_depth=False)
             self.stop()
-            #print("---------------END-----------------")
+            
             self.flag = True
             return
         if(net_gain_loss < 0 and net_gain_loss <= self.maxloss):
-            print("maxloss has reached...")
-            print("SquareOff operation on both contracts call and put begins....")
-            #self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Call",action = "sell",price = "")
-            #self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Put",action = "sell",price = "")
-
+            print("MaxLoss reached...")
+            #print("SquareOff operation on both contracts call and put begins....")
+            
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Call", get_exchange_quotes=True, get_market_depth=False)
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Put", get_exchange_quotes=True, get_market_depth=False)
             self.stop()
-            #print("---------------END-----------------")
+           
             self.flag = True
             return
 
-    def calculate_current(self,product_type,stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution,flag):
+    def calculate_current(self,product_type,stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution,flag):
         
         resultcall = []
         formatted_date = self.get_date_format(expiry_date)
         
         def on_ticks(data):
             
             value = data
             
             if(value['right'] == "Call"):
                 self.currentcall = round(float(value['last']) - float(call_execution), 2)
-                #print(f"P&L (CALL)  : {round(self.currentcall * int(self.quantity),2)}/- Rs")
-                #print("-------------------------------------------------------------------")
+                
                 if(self.flag == False):
-                    self.trigger(product_type, "Call", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution)
+                    self.trigger(product_type, "Call", stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution)
             
             if(value['right'] == "Put"):
                 self.currentput = round(float(value['last']) - float(put_execution), 2)
-                #print(f"P&L (PUT) :  {round(self.currentput * int(self.quantity),2)}/- Rs")
-                #print("-------------------------------------------------------------------")
+                
                 if(self.flag == False):
-                    self.trigger(product_type, "Put", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution)
+                    self.trigger(product_type, "Put", stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution)
             
         self.client.on_ticks = on_ticks
         self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Call", get_exchange_quotes=True, get_market_depth=False)
         self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Put", get_exchange_quotes=True, get_market_depth=False) 
 
         
-    def profit_and_loss(self,product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution):
-        self.calculate_current(product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution, put_execution,False)
+    def profit_and_loss(self,product_type, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution):
+        self.calculate_current(product_type, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution, put_execution,False)
             
-    def long_straddle(self, stock_code, strike_price, qty, expiry_date, stoploss = "", put_price = "0", call_price = "0",product_type = "options", order_type = "market", validity = "day", validity_date = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%S.%fZ'), exchange_code = "NFO"):
+    def straddle(self, strategy_type,stock_code, strike_price, quantity, expiry_date, stoploss = "", put_price = "0", call_price = "0",product_type = "options", order_type = "market", validity = "day", validity_date = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%S.%fZ'), exchange_code = "NFO"):
         
-        self.quantity = qty
+        self.quantity = quantity
+        self.strategy_type = strategy_type
         self.exchange_code = exchange_code 
         self.stock_code = stock_code
         self.product_type = product_type 
         self.expiry_date = expiry_date  
         self.strike_price = strike_price
         self.order_type = order_type
         self.validity = validity
         self.stoploss = stoploss
         #self.quantity = quantity
         self.validity_date = validity_date
+        
+        if(self.socket == 0):
+            self.client.ws_connect()
+            self.socket = 1
+            
+
+        if(strategy_type.lower() not in ["long","short"]):
+            return("strategy_type should be either long or short..")
 
         def place_order_method(stock_code,exchange_code,product,action,order_type,stoploss,quantity,price,validity,validity_date,expiry_date,right,strike_price,res_queue):
          
             data =  self.client.place_order(stock_code=stock_code,
                     exchange_code=exchange_code,
                     product="options",
-                    action = "buy",
+                    action = action,
                     order_type=order_type,
                     stoploss=stoploss,
-                    quantity=qty,
+                    quantity=quantity,
                     price = price,
                     validity= validity,
                     validity_date = validity_date,
                     disclosed_quantity = "0",
                     expiry_date = expiry_date,
                     right= right,
                     strike_price=strike_price)
-            print(data)
-            res_queue.put(data)
+            response = None
+            if(data['Status'] == 200):
+                response = data['Success']['message']
+                print(f"Success : {response} for {right} with order_id :{data['Success']['order_id']}")
+            else:
+                response = data['Error']
+                print(f"Error : {response} for {right}")
+                res_queue.put(data)
             return(data)
                   
         res_queue = queue.Queue()
+        action = "buy"
+
+        if(strategy_type.lower()== "short"):
+            action = "sell"
+        
         #create thread for call and put order to execute simultaneously for buy type
-        t1 = threading.Thread(target = place_order_method,args = (stock_code,exchange_code,"options","buy",order_type,stoploss,qty,call_price,validity,validity_date,expiry_date,"Call",strike_price,res_queue))
+        t1 = threading.Thread(target = place_order_method,args = (stock_code,exchange_code,"options",action,order_type,stoploss,quantity,call_price,validity,validity_date,expiry_date,"Call",strike_price,res_queue))
         t1.start()
         t1.join()
         
         firstresponse = res_queue.get()
         
         res_queue = queue.Queue()
-        t2 = threading.Thread(target = place_order_method,args = (stock_code,exchange_code,"options","buy",order_type,stoploss,qty,put_price,validity,validity_date,expiry_date,"Put",strike_price,res_queue))
+        t2 = threading.Thread(target = place_order_method,args = (stock_code,exchange_code,"options",action,order_type,stoploss,quantity,put_price,validity,validity_date,expiry_date,"Put",strike_price,res_queue))
         t2.start()
         t2.join()
         secondresponse = res_queue.get()
         
         
         #if one of the order fails then cancel the other one which is successfull
         if(firstresponse.get('Status')==200 and secondresponse.get('Status')==500):
@@ -231,15 +253,15 @@
             
         
         else:
             orderids = [] #0th index will contain call order, #1st index will contain put order 
             orderids.append(firstresponse['Success']['order_id']) 
             orderids.append(secondresponse['Success']['order_id'])            
             #define a mechanism to get profit and loss
-            print("----lets wait for 5 seconds for getting the executed status---")
+            print("----Starting live P&L feed...---")
             time.sleep(5)
             details = self.client.get_order_detail(exchange_code=exchange_code,
                         order_id= orderids[0])
 
             call_status = None
             put_status = None
 
@@ -263,14 +285,16 @@
                     put_execution = entry['average_price']
                     put_status = "Executed"
                     self.putexecution = put_execution
                     break
                     
             if(call_execution == -1 or put_execution == -1):
                 print("Dear User order could not execute within time limit ..cancelling it")
+                
+                
                 if(call_execution == -1 and put_execution == -1):
                     print("Both Order Call and Put could not execute to so cancelling it ..... ")
                     self.client.cancel_order(exchange_code=exchange_code,
                     order_id = orderids[0])
                     self.client.cancel_order(exchange_code=exchange_code,
                     order_id = orderids[1])
 
@@ -278,49 +302,55 @@
                     #call cancel order api
                     print("call order could not execute due to some reason so cancelling order")
                     #self.squareoff(self,rightval,exchange_code, stock_code, product_type, expiry_date, right, strike_price, action, order_type, validity, stoploss, quantity, price,validity_date, trade_password, disclosed_quantity)
                     self.client.cancel_order(exchange_code=exchange_code,
                     order_id = orderids[0])
 
                     print("put order is executed squaring off....")
-                    self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Put", action = "sell")
+                    
+                    self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Put")
 
                 elif(put_execution == -1):
                     #call cancel order api
                     print("put order could not execute due to some reason so cancelling order")
                     status = self.client.cancel_order(exchange_code=exchange_code,
                     order_id = orderids[1])
                     print("call order is executed squaring off....")
-                    self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Call", action = "sell")
+                    self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Call")
                     
             else:
                 print("Call order got executed at price :{0} Rs and Put Order got executed at price : {1} Rs".format(call_execution,put_execution))
-                self.profit_and_loss(product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution)
+                self.profit_and_loss(product_type, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution)
             
+    
+    
+    
     def stop(self):
         self.client.ws_disconnect()
+        self.socket = 0
         time.sleep(1)
-        print("squaring off the both contracts and exiting strategy...")
-        square_call = self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Call", action = "sell")
-        square_put = self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Put", action = "sell")
+        print("Squaring off the both contracts and exiting strategy...")
+        print("----------------------------------------")
+        
+        square_call = self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Call")
+        square_put = self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Put")
+        print("----------------------------------------")
         self.create_report(square_call,square_put)
         
 
     def get_pnl(self):
-        #print("- Negative indicates loss")
-        #print(f"P&L (CALL):  {round(self.currentcall*int(self.quantity),2)}/- Rs")
-        #print(f"P&L (PUT):  {round(self.currentput*int(self.quantity),2)}/- Rs")
+        
         outcome = (self.currentcall + self.currentput)*int(self.quantity)
         print(f"P&L (NET) : {round(outcome,2)}/- Rs")
 
-        print("------------------------------------------------------------------------------")
+        print("----------------------------------------")
 
 
     def create_report(self,sq_call,sq_put):
-        print("Report for final P&L...")
+        
         if(sq_call['Status'] == 200 and sq_put['Status'] == 200):
             sq_callid = sq_call["Success"]['order_id']
             sq_putid = sq_put["Success"]['order_id']
 
             print("\nGenerating Final P&L report in 5 seconds....")
             time.sleep(5)
             callrecords = self.client.get_order_detail(exchange_code=self.exchange_code,
```

### Comparing `breeze_strategies-6.0.7/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-6.0.8/breeze_strategies.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze-strategies
-Version: 6.0.7
+Version: 6.0.8
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,28 +17,31 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.7
+pip install breeze_strategies==6.0.8
 
 ```
 
 
 ## code usage
 
 ```python
 
 from breeze_strategies import Strategies
 
 
 obj = Strategies(app_key = "your app key",secret_key = "your secret key",api_session = "your api session",max_profit = "your max profit",max_loss = "your max loss")
-obj.long_straddle(stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
+obj.straddle(strategy_type = "long",stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
+
+obj.straddle(strategy_type = "short",stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
+
 obj.stop() #for disconnection and exit of current strategy
 obj.get_pnl()
 
 ```
```

### Comparing `breeze_strategies-6.0.7/setup.py` & `breeze_strategies-6.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="6.0.7",
+    version="6.0.8",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

