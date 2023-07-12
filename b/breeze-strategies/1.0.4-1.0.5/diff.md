# Comparing `tmp/breeze_strategies-1.0.4.tar.gz` & `tmp/breeze_strategies-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-1.0.4.tar", last modified: Mon Jun 26 08:41:41 2023, max compression
+gzip compressed data, was "breeze_strategies-1.0.5.tar", last modified: Wed Jul 12 06:39:45 2023, max compression
```

## Comparing `breeze_strategies-1.0.4.tar` & `breeze_strategies-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 08:41:41.016701 breeze_strategies-1.0.4/
--rw-rw-rw-   0        0        0     1113 2023-06-23 07:11:33.000000 breeze_strategies-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1543 2023-06-26 08:41:41.013174 breeze_strategies-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      992 2023-06-26 08:41:27.000000 breeze_strategies-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 08:41:40.973175 breeze_strategies-1.0.4/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-1.0.4/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    20393 2023-06-23 09:58:39.000000 breeze_strategies-1.0.4/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:41:41.010174 breeze_strategies-1.0.4/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1543 2023-06-26 08:41:40.000000 breeze_strategies-1.0.4/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-26 08:41:40.000000 breeze_strategies-1.0.4/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 08:41:40.000000 breeze_strategies-1.0.4/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-26 08:41:40.000000 breeze_strategies-1.0.4/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-26 08:41:40.000000 breeze_strategies-1.0.4/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 08:41:41.017697 breeze_strategies-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-06-26 08:41:36.000000 breeze_strategies-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 06:39:45.452181 breeze_strategies-1.0.5/
+-rw-rw-rw-   0        0        0     1113 2023-06-23 07:11:33.000000 breeze_strategies-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1727 2023-07-12 06:39:45.451172 breeze_strategies-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1176 2023-07-12 06:35:15.000000 breeze_strategies-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 06:39:45.397310 breeze_strategies-1.0.5/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-1.0.5/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    28160 2023-07-12 06:39:28.000000 breeze_strategies-1.0.5/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-07-12 06:39:45.448451 breeze_strategies-1.0.5/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1727 2023-07-12 06:39:45.000000 breeze_strategies-1.0.5/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-12 06:39:45.000000 breeze_strategies-1.0.5/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 06:39:45.000000 breeze_strategies-1.0.5/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-12 06:39:45.000000 breeze_strategies-1.0.5/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-12 06:39:45.000000 breeze_strategies-1.0.5/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 06:39:45.452181 breeze_strategies-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-07-12 06:36:35.000000 breeze_strategies-1.0.5/setup.py
```

### Comparing `breeze_strategies-1.0.4/LICENSE` & `breeze_strategies-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-1.0.4/PKG-INFO` & `breeze_strategies-1.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze_strategies
-Version: 1.0.4
+Version: 1.0.5
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
 
-pip install breeze_strategies==1.0.4
+pip install breeze_strategies==1.0.5
 
 ```
 
 ## Updating Library
 
 ```python
 
@@ -50,14 +50,17 @@
 #Execute the strategy
 obj.straddle(strategy_type = "long",
              stock_code = "NIFTY",
              strike_price = "18700",
              quantity = "50",
              expiry_date = "2023-06-29T06:00:00.000Z")
 
+#Execute Single Leg
+obj.single_leg(right = "Call", strategy_type = "short",stock_code = "NIFTY", strike_price = "18700", quantity = "50", expiry_date = "2023-06-29T06:00:00.000Z")
+
 
 #SquareOff existing positions and exit the strategy
 obj.stop() 
 
 
 #Generate Profit & Loss report
 obj.get_pnl()
```

### Comparing `breeze_strategies-1.0.4/README.md` & `breeze_strategies-1.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0.4
+pip install breeze_strategies==1.0.5
 
 ```
 
 ## Updating Library
 
 ```python
 
@@ -34,14 +34,17 @@
 #Execute the strategy
 obj.straddle(strategy_type = "long",
              stock_code = "NIFTY",
              strike_price = "18700",
              quantity = "50",
              expiry_date = "2023-06-29T06:00:00.000Z")
 
+#Execute Single Leg
+obj.single_leg(right = "Call", strategy_type = "short",stock_code = "NIFTY", strike_price = "18700", quantity = "50", expiry_date = "2023-06-29T06:00:00.000Z")
+
 
 #SquareOff existing positions and exit the strategy
 obj.stop() 
 
 
 #Generate Profit & Loss report
 obj.get_pnl()
```

### Comparing `breeze_strategies-1.0.4/breeze_strategies/breeze_strategies.py` & `breeze_strategies-1.0.5/breeze_strategies/breeze_strategies.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         self.validity = ""
         self.stoploss = ""
         self.validity_date = ""
         self.callexecution = ""
         self.putexecution = ""
         self.strategy_type = ""
         self.socket = 0
-    
+        self.right = ""
+
     def squareoff(self,exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, price,validity_date, trade_password, disclosed_quantity,right):
         action = "buy"
         if(self.strategy_type.lower() == "short"):
             action = "buy"
         else:
             action = "sell"
 
@@ -88,72 +89,79 @@
                       }
         year = expiry_date[:4]
         month = expiry_date[5:7]
         day = expiry_date[8:10]
         formatted_date = f"{day}-{month_names[month]}-{year}"
         return(formatted_date)
         
-    def trigger(self,product_type, rightval, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution,put_execution):
+    def trigger(self,product_type, rightval, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution,put_execution,single_leg):
         net_gain_loss = (self.currentcall + self.currentput)*int(quantity)
         print(f"P&L (NET) : {round(net_gain_loss,2)}/- Rs")
         print("----------------------------------------")
         formatted_date = self.get_date_format(expiry_date)
 
         if(net_gain_loss > 0 and net_gain_loss >= self.maxprofit):
             print("TakeProfit reached...")
             #print("SquareOff operation on both contracts call and put begins....")
             
             
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Call", get_exchange_quotes=True, get_market_depth=False)
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Put", get_exchange_quotes=True, get_market_depth=False)
-            self.stop()
+            self.stop(single_leg)
             
             self.flag = True
             return
         if(net_gain_loss < 0 and net_gain_loss <= self.maxloss):
             print("MaxLoss reached...")
             #print("SquareOff operation on both contracts call and put begins....")
             
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Call", get_exchange_quotes=True, get_market_depth=False)
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Put", get_exchange_quotes=True, get_market_depth=False)
-            self.stop()
+            self.stop(single_leg)
            
             self.flag = True
             return
 
-    def calculate_current(self,product_type,stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution,flag):
+    def calculate_current(self,product_type,stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution,single_leg):
         
         resultcall = []
         formatted_date = self.get_date_format(expiry_date)
         
         def on_ticks(data):
             
             value = data
             
             if(value['right'] == "Call"):
                 self.currentcall = round(float(value['last']) - float(call_execution), 2)
                 if(self.strategy_type.lower() == "short"):
                     self.currentcall = self.currentcall*-1
                 if(self.flag == False):
-                    self.trigger(product_type, "Call", stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution)
+                    self.trigger(product_type, "Call", stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution,single_leg)
             
             if(value['right'] == "Put"):
                 self.currentput = round(float(value['last']) - float(put_execution), 2)
                 if(self.strategy_type.lower() == "short"):
                     self.currentput = self.currentput*-1
                 if(self.flag == False):
-                    self.trigger(product_type, "Put", stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution)
+                    self.trigger(product_type, "Put", stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution,single_leg)
             
         self.client.on_ticks = on_ticks
-        self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Call", get_exchange_quotes=True, get_market_depth=False)
-        self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Put", get_exchange_quotes=True, get_market_depth=False) 
+
+        if(single_leg == False):
+            self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Call", get_exchange_quotes=True, get_market_depth=False)
+            self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Put", get_exchange_quotes=True, get_market_depth=False) 
+        else:
+            if(self.right.lower() == "call"):
+                self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Call", get_exchange_quotes=True, get_market_depth=False)
+            else:
+                self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Put", get_exchange_quotes=True, get_market_depth=False) 
 
         
-    def profit_and_loss(self,product_type, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution):
-        self.calculate_current(product_type, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution, put_execution,False)
+    def profit_and_loss(self,product_type, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price,call_execution,put_execution,single_leg = False):
+        self.calculate_current(product_type, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution, put_execution,single_leg)
             
     def straddle(self, strategy_type,stock_code, strike_price, quantity, expiry_date, stoploss = "", put_price = "0", call_price = "0",product_type = "options", order_type = "market", validity = "day", validity_date = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%S.%fZ'), exchange_code = "NFO"):
         
         self.quantity = quantity
         self.strategy_type = strategy_type
         self.exchange_code = exchange_code 
         self.stock_code = stock_code
@@ -319,43 +327,109 @@
                     status = self.client.cancel_order(exchange_code=exchange_code,
                     order_id = orderids[1])
                     print("call order is executed squaring off....")
                     self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Call")
                     
             else:
                 print("Call order got executed at price :{0} Rs and Put Order got executed at price : {1} Rs".format(call_execution,put_execution))
-                self.profit_and_loss(product_type, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution)
+                self.profit_and_loss(product_type, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price,call_execution,put_execution)
             
     
     
     
-    def stop(self):
+    def stop(self,single_leg):
         if(self.socket == 1):
             self.client.ws_disconnect()
         self.socket = 0
         time.sleep(1)
         print("\n")
         print("Squaring off the both contracts and exiting strategy...")
         print("----------------------------------------")
-        
-        square_call = self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Call")
-        square_put = self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Put")
-        print("----------------------------------------")
-        self.create_report(square_call,square_put)
-        
+        if(single_leg == False):
+
+            square_call = self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Call")
+            square_put = self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Put")
+            print("----------------------------------------")
+            self.create_report(square_call,square_put,single_leg)
+        else:
+
+            if(self.right.lower() == "call"):
+                square_call = self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Call")
+                self.create_report(square_call,None,single_leg)
+            else:
+                square_put = self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Put")
+                self.create_report(None,square_put,single_leg)
+
 
     def get_pnl(self):
         
         outcome = (self.currentcall + self.currentput)*int(self.quantity)
         print(f"P&L (NET) : {round(outcome,2)}/- Rs")
 
         print("----------------------------------------")
 
 
-    def create_report(self,sq_call,sq_put):
+    def create_report(self,sq_call,sq_put,single_leg):
+
+        if(single_leg):
+            if(self.right.lower() == "call"):
+                if(sq_call['Status'] == 200):
+                    sq_callid = sq_call["Success"]['order_id']
+                    print("\nGenerating Final P&L report in 5 seconds....")
+                    time.sleep(5)
+                    callrecords = self.client.get_order_detail(exchange_code=self.exchange_code,
+                    order_id= sq_callid)
+
+                    sqcall_price = -1
+                    for record in callrecords['Success']:
+                        if(record['status'] == "Executed"):
+                            sqcall_price = record["average_price"]
+                            break
+                    
+                    plcall = round((float(sqcall_price) - float(self.callexecution))*int(self.quantity),2)
+                    self.currentcall = (float(sqcall_price) - float(self.callexecution))
+
+                    print("----------------------------------------")
+                    print("Profit and Loss Report........")
+                    print(f"P&L (CALL) : {plcall}/- Rs")
+                    
+                    print(f"P&L (NET) : {plcall}/- Rs")
+                    print("----------------------------------------")
+                
+                else:
+                    print("Error : SquareOff for call operation failed.")
+            
+            else:
+                if(sq_put['Status'] == 200):
+                    sq_putid = sq_put["Success"]['order_id']
+                    print("\nGenerating Final P&L report in 5 seconds....")
+                    time.sleep(5)
+                    putrecords = self.client.get_order_detail(exchange_code=self.exchange_code,
+                    order_id= sq_putid)
+
+                    sqput_price = -1
+                    for record in putrecords['Success']:
+                        if(record['status'] == "Executed"):
+                            sqput_price = record["average_price"]
+                            break
+                    
+                    plput = round((float(sqput_price) - float(self.putexecution))*int(self.quantity),2)
+                    self.currentput = (float(sqput_price) - float(self.putexecution))
+
+                    print("----------------------------------------")
+                    print("Profit and Loss Report........")
+                    
+                    print(f"P&L (PUT) : {plput}/- Rs")
+                    print(f"P&L (NET) : {plput}/- Rs")
+                    print("----------------------------------------")
+                
+                else:
+                    print("Error : SquareOff for put operation failed.")
+
+            return
         
         if(sq_call['Status'] == 200 and sq_put['Status'] == 200):
             sq_callid = sq_call["Success"]['order_id']
             sq_putid = sq_put["Success"]['order_id']
 
             print("\nGenerating Final P&L report in 5 seconds....")
             time.sleep(5)
@@ -363,15 +437,15 @@
                         order_id= sq_callid)
 
             putrecords = self.client.get_order_detail(exchange_code=self.exchange_code,
                         order_id= sq_putid)
 
             sqcall_price = -1
             sqput_price = -1
-            time.sleep(5)
+            #time.sleep(5)
             for record in callrecords['Success']:
                 if(record['status'] == "Executed"):
                     sqcall_price = record["average_price"]
                     break
             for record in putrecords["Success"]:
                 if(record['status'] == "Executed"):
                     sqput_price = record["average_price"]
@@ -389,8 +463,92 @@
             print(f"P&L (PUT) : {plput}/- Rs")
             print(f"P&L (NET) : {plput + plcall}/- Rs")
             print("----------------------------------------")
         else:
             print("One of Square off operation failed..")
 
 
+    def single_leg(self,right, strategy_type,stock_code, strike_price, quantity, expiry_date, price = "0", stoploss = "",product_type = "options", order_type = "market", validity = "day", validity_date = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%S.%fZ'), exchange_code = "NFO"):
+        self.quantity = quantity
+        self.strategy_type = strategy_type
+        self.exchange_code = exchange_code 
+        self.stock_code = stock_code
+        self.product_type = product_type 
+        self.expiry_date = expiry_date  
+        self.strike_price = strike_price
+        self.order_type = order_type
+        self.validity = validity
+        self.stoploss = stoploss
+        #self.quantity = quantity
+        self.validity_date = validity_date
+        self.right = right
+
+        action = "buy"
+
+        if(self.strategy_type.lower() == "long"):
+            action = "sell"
+
+
+        data =  self.client.place_order(stock_code=stock_code,
+                    exchange_code=exchange_code,
+                    product="options",
+                    action = action,
+                    order_type=order_type,
+                    stoploss=stoploss,
+                    quantity=quantity,
+                    price = price,
+                    validity= validity,
+                    validity_date = validity_date,
+                    disclosed_quantity = "0",
+                    expiry_date = expiry_date,
+                    right= right,
+                    strike_price=strike_price)
+
+        response = None
+        order_id = None
+        if(data['Status'] == 200):
+            response = data['Success']['message']
+            print(f"Success : {response} for {right} with order_id :{data['Success']['order_id']}") 
+            order_id = data['Success']['order_id']      
+        
+        else:
+            response = data['Error']
+            print(f"Error : {response} for {right}")
+
+        if(order_id!=None):
+            print("\n")
+            print("----Starting live P&L feed...---")
+            time.sleep(5)
+            details = self.client.get_order_detail(exchange_code=exchange_code,
+                        order_id= order_id)
+
+            #execution_price = -1
+            
+            
+            #print(f"order ids are : {orderids}")
+            call_execution = "0"
+            put_execution = "0"
+
+            for entry in details['Success']:
+                if(entry['status'] == "Executed"):
+                    execution = entry['average_price']
+                    #call_status = "Executed"
+                    if(right.lower() == "call"):
+                        call_execution = execution
+                        self.callexecution = execution
+                        break
+                    else:
+                        put_execution = execution
+                        self.putexecution = execution
+                        break
+
+        self.profit_and_loss(product_type, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price,call_execution,put_execution,True)
+
+            
+
+            
+
+
+
+
+
```

### Comparing `breeze_strategies-1.0.4/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-1.0.5/breeze_strategies.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze-strategies
-Version: 1.0.4
+Version: 1.0.5
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
 
-pip install breeze_strategies==1.0.4
+pip install breeze_strategies==1.0.5
 
 ```
 
 ## Updating Library
 
 ```python
 
@@ -50,14 +50,17 @@
 #Execute the strategy
 obj.straddle(strategy_type = "long",
              stock_code = "NIFTY",
              strike_price = "18700",
              quantity = "50",
              expiry_date = "2023-06-29T06:00:00.000Z")
 
+#Execute Single Leg
+obj.single_leg(right = "Call", strategy_type = "short",stock_code = "NIFTY", strike_price = "18700", quantity = "50", expiry_date = "2023-06-29T06:00:00.000Z")
+
 
 #SquareOff existing positions and exit the strategy
 obj.stop() 
 
 
 #Generate Profit & Loss report
 obj.get_pnl()
```

### Comparing `breeze_strategies-1.0.4/setup.py` & `breeze_strategies-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="1.0.4",
+    version="1.0.5",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

