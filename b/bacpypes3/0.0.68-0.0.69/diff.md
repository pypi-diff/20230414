# Comparing `tmp/bacpypes3-0.0.68-py3-none-any.whl.zip` & `tmp/bacpypes3-0.0.69-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 273235 bytes, number of entries: 97
--rw-rw-r--  2.0 unx     1370 b- defN 23-Apr-07 19:15 bacpypes3/__init__.py
+Zip file size: 273293 bytes, number of entries: 97
+-rw-rw-r--  2.0 unx     1370 b- defN 23-Apr-14 14:19 bacpypes3/__init__.py
 -rw-rw-r--  2.0 unx    22682 b- defN 23-Apr-03 19:06 bacpypes3/__main__.py
 -rw-rw-r--  2.0 unx    56648 b- defN 23-Jan-24 05:27 bacpypes3/apdu.py
 -rw-rw-r--  2.0 unx    32984 b- defN 23-Apr-03 19:01 bacpypes3/app.py
 -rw-rw-r--  2.0 unx    65777 b- defN 23-Apr-04 12:53 bacpypes3/appservice.py
 -rw-rw-r--  2.0 unx    21553 b- defN 23-Mar-22 18:04 bacpypes3/argparse.py
 -rw-rw-r--  2.0 unx   106747 b- defN 23-Apr-03 19:42 bacpypes3/basetypes.py
 -rw-rw-r--  2.0 unx    16150 b- defN 23-Apr-03 15:32 bacpypes3/cmd.py
 -rw-rw-r--  2.0 unx     7934 b- defN 22-Nov-21 19:40 bacpypes3/comm.py
 -rw-rw-r--  2.0 unx     7128 b- defN 23-Jan-24 05:27 bacpypes3/console.py
 -rw-rw-r--  2.0 unx    64295 b- defN 23-Apr-07 19:15 bacpypes3/constructeddata.py
 -rw-rw-r--  2.0 unx    10883 b- defN 23-Jan-24 13:27 bacpypes3/debugging.py
 -rw-rw-r--  2.0 unx     9685 b- defN 23-Feb-08 13:29 bacpypes3/errors.py
--rw-rw-r--  2.0 unx    75702 b- defN 23-Apr-03 14:58 bacpypes3/netservice.py
+-rw-rw-r--  2.0 unx    76370 b- defN 23-Apr-14 14:22 bacpypes3/netservice.py
 -rw-rw-r--  2.0 unx    28240 b- defN 23-Jan-24 05:27 bacpypes3/npdu.py
 -rw-rw-r--  2.0 unx    93859 b- defN 23-Apr-04 12:10 bacpypes3/object.py
 -rw-rw-r--  2.0 unx    64688 b- defN 23-Feb-15 17:04 bacpypes3/pdu.py
 -rw-rw-r--  2.0 unx    80966 b- defN 23-Feb-17 06:25 bacpypes3/primitivedata.py
 -rw-rw-r--  2.0 unx     3884 b- defN 23-Jan-27 13:49 bacpypes3/settings.py
 -rw-rw-r--  2.0 unx     9099 b- defN 23-Jan-09 14:29 bacpypes3/ipv4/__init__.py
 -rw-rw-r--  2.0 unx     8795 b- defN 23-Mar-23 15:36 bacpypes3/ipv4/app.py
@@ -88,12 +88,12 @@
 -rw-rw-r--  2.0 unx     3588 b- defN 21-Jun-28 12:37 tests/test_primitive_data/test_unsigned.py
 -rw-rw-r--  2.0 unx      130 b- defN 23-Jan-26 13:59 tests/test_utilities/__init__.py
 -rw-rw-r--  2.0 unx    18594 b- defN 23-Jan-26 13:59 tests/test_utilities/test_state_machine.py
 -rw-rw-r--  2.0 unx      200 b- defN 23-Jan-26 13:59 tests/test_vlan/__init__.py
 -rw-rw-r--  2.0 unx     8287 b- defN 23-Jan-26 13:59 tests/test_vlan/test_ipv4_network.py
 -rw-rw-r--  2.0 unx     6304 b- defN 23-Jan-26 13:59 tests/test_vlan/test_ipv4_router.py
 -rw-rw-r--  2.0 unx     8904 b- defN 23-Jan-26 13:59 tests/test_vlan/test_network.py
--rw-rw-r--  2.0 unx      649 b- defN 23-Apr-07 20:20 bacpypes3-0.0.68.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-07 20:20 bacpypes3-0.0.68.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Apr-07 20:20 bacpypes3-0.0.68.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     8257 b- defN 23-Apr-07 20:20 bacpypes3-0.0.68.dist-info/RECORD
-97 files, 1455563 bytes uncompressed, 260293 bytes compressed:  82.1%
+-rw-rw-r--  2.0 unx      649 b- defN 23-Apr-14 14:24 bacpypes3-0.0.69.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-14 14:24 bacpypes3-0.0.69.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Apr-14 14:24 bacpypes3-0.0.69.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     8257 b- defN 23-Apr-14 14:24 bacpypes3-0.0.69.dist-info/RECORD
+97 files, 1456231 bytes uncompressed, 260351 bytes compressed:  82.1%
```

## zipnote {}

```diff
@@ -273,20 +273,20 @@
 
 Filename: tests/test_vlan/test_ipv4_router.py
 Comment: 
 
 Filename: tests/test_vlan/test_network.py
 Comment: 
 
-Filename: bacpypes3-0.0.68.dist-info/METADATA
+Filename: bacpypes3-0.0.69.dist-info/METADATA
 Comment: 
 
-Filename: bacpypes3-0.0.68.dist-info/WHEEL
+Filename: bacpypes3-0.0.69.dist-info/WHEEL
 Comment: 
 
-Filename: bacpypes3-0.0.68.dist-info/top_level.txt
+Filename: bacpypes3-0.0.69.dist-info/top_level.txt
 Comment: 
 
-Filename: bacpypes3-0.0.68.dist-info/RECORD
+Filename: bacpypes3-0.0.69.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bacpypes3/__init__.py

```diff
@@ -14,15 +14,15 @@
 if _sys.platform not in _supported_platforms:
     _warnings.warn("unsupported platform", RuntimeWarning)
 
 #
 #   Project Metadata
 #
 
-__version__ = "0.0.68"
+__version__ = "0.0.69"
 __author__ = "Joel Bender"
 __email__ = "joel@carrickbender.com"
 
 #
 #   Settings and Debugging
 #
```

## bacpypes3/netservice.py

```diff
@@ -103,15 +103,19 @@
 
 @bacpypes_debugging
 class RouterInfoCache(DebugContents):
     """
     This class provides an in-memory implementation of a database of RouterInfo
     objects.
     """
-    _debug_contents = ('routers+', 'path_info+',)
+
+    _debug_contents = (
+        "routers+",
+        "path_info+",
+    )
     _debug: Callable[..., None]
 
     routers: Dict[Optional[int], Dict[Address, RouterInfo]]
     path_info: Dict[Tuple[Optional[int], int], RouterInfo]
 
     def __init__(self):
         if _debug:
@@ -294,15 +298,14 @@
 #
 #   NetworkAdapter
 #
 
 
 @bacpypes_debugging
 class NetworkAdapter(Client[PDU], DebugContents):
-
     _debug: Callable[..., None]
     _debug_contents = (
         "adapterSAP-",
         "adapterNet",
         "adapterAddr",
         "adapterNetConfigured",
     )
@@ -386,15 +389,14 @@
 #
 #   NetworkServiceAccessPoint
 #
 
 
 @bacpypes_debugging
 class NetworkServiceAccessPoint(ServiceAccessPoint, Server[PDU], DebugContents):
-
     _debug: Callable[..., None]
     _warning: Callable[..., None]
     _debug_contents = (
         "adapters++",
         "local_adapter-",
         "router_info_cache",
     )
@@ -672,16 +674,22 @@
 
         else:
             if _debug:
                 NetworkServiceAccessPoint._debug("    - look for the router")
 
             result_list = await nse.who_is_router_to_network(network=dnet)
             if not result_list:
+                if _debug:
+                    NetworkServiceAccessPoint._debug("    - no router responded")
                 raise UnknownRoute()
             if len(result_list) > 1:
+                if _debug:
+                    NetworkServiceAccessPoint._debug(
+                        "    - more than one router responded"
+                    )
                 raise UnknownRoute()
 
             router_adapter, i_am_router_to_network = result_list[0]
             if _debug:
                 NetworkServiceAccessPoint._debug(
                     "    - found path: %r, %r",
                     router_adapter,
@@ -1031,15 +1039,17 @@
         self,
         nse: NetworkServiceElement,
         adapter: Optional[NetworkAdapter] = None,
         router_address: Optional[Address] = None,
         network: Optional[int] = None,
     ) -> None:
         if _debug:
-            WhoIsRouterToNetworkFuture._debug("__init__ %r %r", nse, network)
+            WhoIsRouterToNetworkFuture._debug(
+                "__init__ %r %r %r %r", nse, adapter, router_address, network
+            )
 
         self.nse = nse
         self.adapter = adapter
         self.router_address = router_address
         self.network = network
 
         self.result_list = []
@@ -1079,15 +1089,22 @@
             npdu_source = npdu.npduSADR
             npdu_source.addrRoute = npdu.pduSource
         else:
             npdu_source = npdu.pduSource
         if _debug:
             WhoIsRouterToNetworkFuture._debug("    - npdu_source: %r", npdu_source)
 
-        if not self.router_address:
+        if self.network is not None:
+            if self.network in npdu.iartnNetworkList:
+                if _debug:
+                    WhoIsRouterToNetworkFuture._debug("    - network match")
+                self.result_list.append((adapter, npdu))
+                self.future.set_result(self.result_list)
+
+        elif not self.router_address:
             if _debug:
                 WhoIsRouterToNetworkFuture._debug("    - wildcard match")
             self.result_list.append((adapter, npdu))
 
         elif npdu_source.match(self.router_address):
             if _debug:
                 WhoIsRouterToNetworkFuture._debug("    - address match")
@@ -1245,15 +1262,14 @@
             InitializeRoutingTableFuture._debug("timeout")
 
         self.future.set_result(self.result_list)
 
 
 @bacpypes_debugging
 class NetworkServiceElement(ApplicationServiceElement, DebugContents):
-
     _debug: Callable[..., None]
     _debug_contents: Tuple[str, ...] = (
         "who_is_router_to_network_futures",
         "router_to_network_resolution",
         "what_is_network_number_resolution",
     )
```

## Comparing `bacpypes3-0.0.68.dist-info/METADATA` & `bacpypes3-0.0.69.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacpypes3
-Version: 0.0.68
+Version: 0.0.69
 Summary: BACnet Communications Library
 Home-page: https://github.com/JoelBender/bacpypes3
 Author: Joel Bender
 Author-email: joel@carrickbender.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

## Comparing `bacpypes3-0.0.68.dist-info/RECORD` & `bacpypes3-0.0.69.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-bacpypes3/__init__.py,sha256=pSCoUKRhPu9wceyedLdM5tY3kbKFhL769s0E9yCca0M,1370
+bacpypes3/__init__.py,sha256=csA54UC44778jTo64fgEww_32SMnEd6hXPYfH7eI5pY,1370
 bacpypes3/__main__.py,sha256=cSGqfoxjQT2Jv3fd435oC7knne7oLM4JKBoQIg3fH6g,22682
 bacpypes3/apdu.py,sha256=4v7ue43Qux1agAebfCglhkdb_DZAVSQ-4J-29c-UfEk,56648
 bacpypes3/app.py,sha256=brRei_JuuV1M1T7L3QZO1sk-_nDb_FFPPZk90Gy5G98,32984
 bacpypes3/appservice.py,sha256=Mroubx8ZBpAAg8wwfxfvcMIkNQ5aXQ0RtRBARXwGViI,65777
 bacpypes3/argparse.py,sha256=Hi0CHD8ILFBesZ3gJ3XRJ_B5lW70alBs5XbOByacRaE,21553
 bacpypes3/basetypes.py,sha256=o0DQTAyod8NBGAMoDXGnEnMXZ_sZCCl-taro5B_MqUU,106747
 bacpypes3/cmd.py,sha256=R57uI1p5bj1Ixr57HJfVpL1VqwfCYlzx41xIWApm3qE,16150
 bacpypes3/comm.py,sha256=trZC92o41mfEMlUGT69PpBPowfyzBiObvEHY6J4cU8E,7934
 bacpypes3/console.py,sha256=fCLUgiK1ZwkckYGCD6zp8Sx9vienIVPTvLDbY8XeTbY,7128
 bacpypes3/constructeddata.py,sha256=dDRn_EhuQkBjZZd-X_xXE03dVtpudYGyQ7pRS4SeaHM,64295
 bacpypes3/debugging.py,sha256=1HgJT7XZi2OOs-pC0gOpLPFawVKi6ZPQJLl3lm2WrI8,10883
 bacpypes3/errors.py,sha256=C2a1lmTi6K76at32GDy8ioRadFxdHyAOkakGN2u6cwk,9685
-bacpypes3/netservice.py,sha256=Sb_Fb_DH62ka1-QlSKyvMwB9W3Xw_B5nQcWiit7NUzg,75702
+bacpypes3/netservice.py,sha256=F5mjuC7AKeQ3pYPeudQFbT6Aa7KblqrxdHTjuz-sFgQ,76370
 bacpypes3/npdu.py,sha256=HjK5WNjZbQlaRL20qpQ8Q8AW3sDOtJ1ycU67ePV6rQE,28240
 bacpypes3/object.py,sha256=ig9zfn8kxMjdk46X2IQP1hl74yRV5YL3lQRou5GghoI,93859
 bacpypes3/pdu.py,sha256=Td7XV60rlwso_rhn4rKpsBE5KAB-NlQn5CCfUrzc3bY,64688
 bacpypes3/primitivedata.py,sha256=y7g3dbTJp9Szk04oSyQ6XujhTroYFm1jPpECULDvKaw,80966
 bacpypes3/settings.py,sha256=lBMeaIsqqjd7Gu0S5gEtC3m5snUIgATABPCKsywFfTQ,3884
 bacpypes3/ipv4/__init__.py,sha256=uQU3qI8z5eve1r6jrm58O2em7yRYPFnvQXLQXg70Pvo,9099
 bacpypes3/ipv4/app.py,sha256=cn__EqCZG0I4a2iNJOziVDhq_P7aXFm_Pv2t2DOZ0nI,8795
@@ -87,11 +87,11 @@
 tests/test_primitive_data/test_unsigned.py,sha256=SVhoVpBRgP48Apklv_QCYNzYv315Mniat6lOB1qGF7A,3588
 tests/test_utilities/__init__.py,sha256=81GA1pRdx-3CmJWAjPz1UNjR1keklu_tMI1H1OvXdUM,130
 tests/test_utilities/test_state_machine.py,sha256=ex0ZxsNo-r_LvNmEJHGoc6kntaYfrOIPgOVEo7X4A5k,18594
 tests/test_vlan/__init__.py,sha256=gELFXeqGnaJYTSf5Y95zyULdCATaDu5QDypYTAmOhZs,200
 tests/test_vlan/test_ipv4_network.py,sha256=boUotVyuiP30f4JosObeZfFA_82_wFRp3wBH9VNXMAg,8287
 tests/test_vlan/test_ipv4_router.py,sha256=7W9kNJ5qT63jV6FcHwNQfv3fu_LaZwTEbjlKXQSLHkM,6304
 tests/test_vlan/test_network.py,sha256=3qVingOmGHdZWVwNJz5GfANmhRJ-DY9Xa1N87Y-boSY,8904
-bacpypes3-0.0.68.dist-info/METADATA,sha256=6b7o-Q0lhK7l3af1NqdtF03_FKJtZDLnfWKp3_RhlHM,649
-bacpypes3-0.0.68.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-bacpypes3-0.0.68.dist-info/top_level.txt,sha256=7Dm99jRUNc7RMdEbDzHTP950Pc1F6gBv_SHMeRT5nBA,16
-bacpypes3-0.0.68.dist-info/RECORD,,
+bacpypes3-0.0.69.dist-info/METADATA,sha256=7hRjPczlvVtTYBkW4Umao8yLsMVRaB_XfWTt-H9pg3I,649
+bacpypes3-0.0.69.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+bacpypes3-0.0.69.dist-info/top_level.txt,sha256=7Dm99jRUNc7RMdEbDzHTP950Pc1F6gBv_SHMeRT5nBA,16
+bacpypes3-0.0.69.dist-info/RECORD,,
```

