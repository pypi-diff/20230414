# Comparing `tmp/shipday-1.1.4.tar.gz` & `tmp/shipday-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipday-1.1.4.tar", last modified: Thu Apr  6 10:40:31 2023, max compression
+gzip compressed data, was "shipday-1.2.0.tar", last modified: Fri Apr 14 18:52:40 2023, max compression
```

## Comparing `shipday-1.1.4.tar` & `shipday-1.2.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-06 10:40:31.139137 shipday-1.1.4/
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     6087 2023-04-06 10:40:31.138968 shipday-1.1.4/PKG-INFO
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     5027 2022-08-28 13:52:12.000000 shipday-1.1.4/README.md
--rw-r--r--   0 shahriartanvir   (501) staff       (20)       38 2023-04-06 10:40:31.139195 shipday-1.1.4/setup.cfg
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     2199 2022-12-29 20:00:12.000000 shipday-1.1.4/setup.py
-drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-06 10:40:31.130250 shipday-1.1.4/shipday/
--rw-r--r--   0 shahriartanvir   (501) staff       (20)       43 2022-08-01 08:56:51.000000 shipday-1.1.4/shipday/__init__.py
-drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-06 10:40:31.131724 shipday-1.1.4/shipday/carrier/
--rw-r--r--   0 shahriartanvir   (501) staff       (20)       59 2022-08-01 11:43:29.000000 shipday-1.1.4/shipday/carrier/__init__.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     1704 2022-08-08 11:43:06.000000 shipday-1.1.4/shipday/carrier/carrier_request.py
-drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-06 10:40:31.132273 shipday-1.1.4/shipday/exeptions/
--rw-r--r--   0 shahriartanvir   (501) staff       (20)       64 2022-08-02 14:22:05.000000 shipday-1.1.4/shipday/exeptions/__init__.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)      129 2022-08-02 14:28:09.000000 shipday-1.1.4/shipday/exeptions/shipday_exeption.py
-drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-06 10:40:31.132674 shipday-1.1.4/shipday/httpclient/
--rw-r--r--   0 shahriartanvir   (501) staff       (20)        0 2022-08-01 09:04:25.000000 shipday-1.1.4/shipday/httpclient/__init__.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     1408 2022-08-18 16:20:10.000000 shipday-1.1.4/shipday/httpclient/shipdayclient.py
-drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-06 10:40:31.136597 shipday-1.1.4/shipday/order/
--rw-r--r--   0 shahriartanvir   (501) staff       (20)      363 2022-08-08 13:53:26.000000 shipday-1.1.4/shipday/order/__init__.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     2811 2022-12-29 19:56:44.000000 shipday-1.1.4/shipday/order/address.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)      160 2022-08-02 04:19:29.000000 shipday-1.1.4/shipday/order/card_type.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     2412 2022-08-09 11:08:05.000000 shipday-1.1.4/shipday/order/customer.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     2346 2022-08-08 15:01:50.000000 shipday-1.1.4/shipday/order/order_cost.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     5825 2023-04-06 10:24:46.000000 shipday-1.1.4/shipday/order/order_info.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     2710 2023-04-06 10:24:46.000000 shipday-1.1.4/shipday/order/order_item.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     4011 2022-08-09 12:06:24.000000 shipday-1.1.4/shipday/order/order_query.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)      608 2022-08-09 11:55:38.000000 shipday-1.1.4/shipday/order/order_status.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     2106 2022-08-08 14:10:17.000000 shipday-1.1.4/shipday/order/pickup.py
-drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-06 10:40:31.137942 shipday-1.1.4/shipday/services/
--rw-r--r--   0 shahriartanvir   (501) staff       (20)      196 2022-08-18 08:55:56.000000 shipday-1.1.4/shipday/services/__init__.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)      915 2022-08-26 05:35:26.000000 shipday-1.1.4/shipday/services/carrier_service.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     3303 2023-03-29 16:35:29.000000 shipday-1.1.4/shipday/services/on_demand_delivery_service.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     2395 2022-08-03 14:35:20.000000 shipday-1.1.4/shipday/services/order_service.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)      618 2022-08-18 08:57:10.000000 shipday-1.1.4/shipday/shipday_object.py
-drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-06 10:40:31.138479 shipday-1.1.4/shipday/utils/
--rw-r--r--   0 shahriartanvir   (501) staff       (20)        0 2022-08-01 15:47:51.000000 shipday-1.1.4/shipday/utils/__init__.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)      907 2022-08-18 16:48:27.000000 shipday-1.1.4/shipday/utils/verifiers.py
--rw-r--r--   0 shahriartanvir   (501) staff       (20)       18 2023-04-06 10:24:46.000000 shipday-1.1.4/shipday/version.py
-drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-06 10:40:31.131171 shipday-1.1.4/shipday.egg-info/
--rw-r--r--   0 shahriartanvir   (501) staff       (20)     6087 2023-04-06 10:40:31.000000 shipday-1.1.4/shipday.egg-info/PKG-INFO
--rw-r--r--   0 shahriartanvir   (501) staff       (20)      905 2023-04-06 10:40:31.000000 shipday-1.1.4/shipday.egg-info/SOURCES.txt
--rw-r--r--   0 shahriartanvir   (501) staff       (20)        1 2023-04-06 10:40:31.000000 shipday-1.1.4/shipday.egg-info/dependency_links.txt
--rw-r--r--   0 shahriartanvir   (501) staff       (20)       43 2023-04-06 10:40:31.000000 shipday-1.1.4/shipday.egg-info/requires.txt
--rw-r--r--   0 shahriartanvir   (501) staff       (20)        8 2023-04-06 10:40:31.000000 shipday-1.1.4/shipday.egg-info/top_level.txt
+drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-14 18:52:40.785620 shipday-1.2.0/
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     6087 2023-04-14 18:52:40.785486 shipday-1.2.0/PKG-INFO
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     5027 2022-08-28 13:52:12.000000 shipday-1.2.0/README.md
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)       38 2023-04-14 18:52:40.785668 shipday-1.2.0/setup.cfg
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     2199 2022-12-29 20:00:12.000000 shipday-1.2.0/setup.py
+drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-14 18:52:40.778345 shipday-1.2.0/shipday/
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)       43 2022-08-01 08:56:51.000000 shipday-1.2.0/shipday/__init__.py
+drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-14 18:52:40.779517 shipday-1.2.0/shipday/carrier/
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)       59 2022-08-01 11:43:29.000000 shipday-1.2.0/shipday/carrier/__init__.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     1704 2022-08-08 11:43:06.000000 shipday-1.2.0/shipday/carrier/carrier_request.py
+drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-14 18:52:40.780007 shipday-1.2.0/shipday/exeptions/
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)       64 2022-08-02 14:22:05.000000 shipday-1.2.0/shipday/exeptions/__init__.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)      129 2022-08-02 14:28:09.000000 shipday-1.2.0/shipday/exeptions/shipday_exeption.py
+drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-14 18:52:40.780342 shipday-1.2.0/shipday/httpclient/
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)        0 2022-08-01 09:04:25.000000 shipday-1.2.0/shipday/httpclient/__init__.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     1408 2022-08-18 16:20:10.000000 shipday-1.2.0/shipday/httpclient/shipdayclient.py
+drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-14 18:52:40.783504 shipday-1.2.0/shipday/order/
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)      363 2022-08-08 13:53:26.000000 shipday-1.2.0/shipday/order/__init__.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     2811 2022-12-29 19:56:44.000000 shipday-1.2.0/shipday/order/address.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)      160 2022-08-02 04:19:29.000000 shipday-1.2.0/shipday/order/card_type.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     2412 2022-08-09 11:08:05.000000 shipday-1.2.0/shipday/order/customer.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     2346 2022-08-08 15:01:50.000000 shipday-1.2.0/shipday/order/order_cost.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     6358 2023-04-06 10:47:14.000000 shipday-1.2.0/shipday/order/order_info.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     2710 2023-04-06 10:47:14.000000 shipday-1.2.0/shipday/order/order_item.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     4011 2022-08-09 12:06:24.000000 shipday-1.2.0/shipday/order/order_query.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)      608 2022-08-09 11:55:38.000000 shipday-1.2.0/shipday/order/order_status.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     2106 2022-08-08 14:10:17.000000 shipday-1.2.0/shipday/order/pickup.py
+drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-14 18:52:40.784782 shipday-1.2.0/shipday/services/
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)      196 2022-08-18 08:55:56.000000 shipday-1.2.0/shipday/services/__init__.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)      915 2022-08-26 05:35:26.000000 shipday-1.2.0/shipday/services/carrier_service.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     3303 2023-03-29 16:35:29.000000 shipday-1.2.0/shipday/services/on_demand_delivery_service.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     2395 2022-08-03 14:35:20.000000 shipday-1.2.0/shipday/services/order_service.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)      618 2022-08-18 08:57:10.000000 shipday-1.2.0/shipday/shipday_object.py
+drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-14 18:52:40.785191 shipday-1.2.0/shipday/utils/
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)        0 2022-08-01 15:47:51.000000 shipday-1.2.0/shipday/utils/__init__.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)      907 2022-08-18 16:48:27.000000 shipday-1.2.0/shipday/utils/verifiers.py
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)       18 2023-04-06 10:44:56.000000 shipday-1.2.0/shipday/version.py
+drwxr-xr-x   0 shahriartanvir   (501) staff       (20)        0 2023-04-14 18:52:40.779102 shipday-1.2.0/shipday.egg-info/
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)     6087 2023-04-14 18:52:40.000000 shipday-1.2.0/shipday.egg-info/PKG-INFO
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)      905 2023-04-14 18:52:40.000000 shipday-1.2.0/shipday.egg-info/SOURCES.txt
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)        1 2023-04-14 18:52:40.000000 shipday-1.2.0/shipday.egg-info/dependency_links.txt
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)       43 2023-04-14 18:52:40.000000 shipday-1.2.0/shipday.egg-info/requires.txt
+-rw-r--r--   0 shahriartanvir   (501) staff       (20)        8 2023-04-14 18:52:40.000000 shipday-1.2.0/shipday.egg-info/top_level.txt
```

### Comparing `shipday-1.1.4/PKG-INFO` & `shipday-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipday
-Version: 1.1.4
+Version: 1.2.0
 Summary: Python library for Shipday API
 Home-page: https://shipday.com/
 Author: Shipday
 Author-email: shahriar@shipday.com
 License: MIT
 Keywords: Shipday,DoorDash,Uber,Delivery API,Dispatch API,DoorDash API,Uber API,Dispatch App,Courier App,Delivery Dispatch,Delivery integration,Delivery Management,Dispatch Management,Delivery Service Integration,Local Delivery API
 Platform: UNKNOWN
```

### Comparing `shipday-1.1.4/README.md` & `shipday-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/setup.py` & `shipday-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday/carrier/carrier_request.py` & `shipday-1.2.0/shipday/carrier/carrier_request.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday/httpclient/shipdayclient.py` & `shipday-1.2.0/shipday/httpclient/shipdayclient.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday/order/address.py` & `shipday-1.2.0/shipday/order/address.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday/order/customer.py` & `shipday-1.2.0/shipday/order/customer.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday/order/order_cost.py` & `shipday-1.2.0/shipday/order/order_cost.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday/order/order_info.py` & `shipday-1.2.0/shipday/order/order_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         self._customer: Customer = customer or Customer(**kwargs)
         self._pickup: Pickup = pickup or Pickup(**kwargs)
         self._order_items: List[OrderItem] = order_items or list(
             map(lambda item: OrderItem(**item), kwargs['orderItems'] or []))
         self._order_cost: OrderCost = order_cost or OrderCost(**kwargs)
         self._delivery_time: datetime = expected_delivery_time
         self._pickup_time: datetime = expected_pickup_time
+        self._delivery_instruction = kwargs['deliveryInstruction'] or kwargs['delivery_instruction']
 
     @property
     def order_number(self) -> str:
         return self._order_number
 
     @order_number.setter
     def order_number(self, value: str):
@@ -104,14 +105,23 @@
         return self._pickup_time
 
     @expected_pickup_time.setter
     def expected_pickup_time(self, value):
         verify_none_or_instance_of(datetime, value, 'Pickup time is not of type ' + str(datetime))
         self._pickup_time = value
 
+    @property
+    def delivery_instruction(self):
+        return self._delivery_instruction
+
+    @delivery_instruction.setter
+    def delivery_instruction(self, value: str):
+        verify_none_or_instance_of(str, value, 'Delivery Instruction must be of type string')
+        self._delivery_instruction = value
+
     def __repr__(self):
         self.get_body()
 
     def update_total_cost(self):
         total = self._order_cost.tax + self._order_cost.tips + self._order_cost.delivery_fee - self._order_cost.discount
         try:
             for item in self.order_items:
@@ -150,8 +160,11 @@
         if self.expected_delivery_time is not None:
             obj['expectedDeliveryDate'] = self.expected_delivery_time.date().isoformat()
             obj['expectedDeliveryTime'] = self.expected_delivery_time.time().isoformat(timespec='seconds')
 
         if self.expected_pickup_time is not None:
             obj['expectedPickupTime'] = self.expected_pickup_time.time().isoformat(timespec='seconds')
 
+        if self._delivery_instruction is not None:
+            obj['deliveryInstruction'] = self._delivery_instruction
+
         return obj
```

### Comparing `shipday-1.1.4/shipday/order/order_item.py` & `shipday-1.2.0/shipday/order/order_item.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday/order/order_query.py` & `shipday-1.2.0/shipday/order/order_query.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday/order/order_status.py` & `shipday-1.2.0/shipday/order/order_status.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday/order/pickup.py` & `shipday-1.2.0/shipday/order/pickup.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday/services/carrier_service.py` & `shipday-1.2.0/shipday/services/carrier_service.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday/services/on_demand_delivery_service.py` & `shipday-1.2.0/shipday/services/on_demand_delivery_service.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday/services/order_service.py` & `shipday-1.2.0/shipday/services/order_service.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday/shipday_object.py` & `shipday-1.2.0/shipday/shipday_object.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday/utils/verifiers.py` & `shipday-1.2.0/shipday/utils/verifiers.py`

 * *Files identical despite different names*

### Comparing `shipday-1.1.4/shipday.egg-info/PKG-INFO` & `shipday-1.2.0/shipday.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipday
-Version: 1.1.4
+Version: 1.2.0
 Summary: Python library for Shipday API
 Home-page: https://shipday.com/
 Author: Shipday
 Author-email: shahriar@shipday.com
 License: MIT
 Keywords: Shipday,DoorDash,Uber,Delivery API,Dispatch API,DoorDash API,Uber API,Dispatch App,Courier App,Delivery Dispatch,Delivery integration,Delivery Management,Dispatch Management,Delivery Service Integration,Local Delivery API
 Platform: UNKNOWN
```

### Comparing `shipday-1.1.4/shipday.egg-info/SOURCES.txt` & `shipday-1.2.0/shipday.egg-info/SOURCES.txt`

 * *Files identical despite different names*

