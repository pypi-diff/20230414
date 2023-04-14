# Comparing `tmp/nso-oc-2.43.2.tar.gz` & `tmp/nso-oc-2.44.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.43.2.tar", last modified: Thu Apr 13 18:04:36 2023, max compression
+gzip compressed data, was "nso-oc-2.44.0.tar", last modified: Fri Apr 14 13:48:34 2023, max compression
```

## Comparing `nso-oc-2.43.2.tar` & `nso-oc-2.44.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:36.440905 nso-oc-2.43.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-13 18:03:59.000000 nso-oc-2.43.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-13 18:03:59.000000 nso-oc-2.43.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-13 18:04:36.440905 nso-oc-2.43.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-13 18:03:59.000000 nso-oc-2.43.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:36.436905 nso-oc-2.43.2/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-13 18:04:36.000000 nso-oc-2.43.2/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-13 18:04:36.000000 nso-oc-2.43.2/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:04:36.000000 nso-oc-2.43.2/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 18:04:36.000000 nso-oc-2.43.2/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 18:04:36.000000 nso-oc-2.43.2/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 18:04:36.000000 nso-oc-2.43.2/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:36.436905 nso-oc-2.43.2/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:36.440905 nso-oc-2.43.2/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    58208 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    41835 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    38030 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29451 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)    90722 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:36.440905 nso-oc-2.43.2/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 18:03:59.000000 nso-oc-2.43.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 18:04:36.440905 nso-oc-2.43.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-13 18:03:59.000000 nso-oc-2.43.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:48:34.706246 nso-oc-2.44.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-14 13:48:08.000000 nso-oc-2.44.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 13:48:08.000000 nso-oc-2.44.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-14 13:48:34.706246 nso-oc-2.44.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-14 13:48:08.000000 nso-oc-2.44.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:48:34.702246 nso-oc-2.44.0/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-14 13:48:34.000000 nso-oc-2.44.0/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-14 13:48:34.000000 nso-oc-2.44.0/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:48:34.000000 nso-oc-2.44.0/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 13:48:34.000000 nso-oc-2.44.0/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 13:48:34.000000 nso-oc-2.44.0/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 13:48:34.000000 nso-oc-2.44.0/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:48:34.702246 nso-oc-2.44.0/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:48:34.706246 nso-oc-2.44.0/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58208 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49391 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38030 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29451 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90722 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:48:34.706246 nso-oc-2.44.0/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 13:48:08.000000 nso-oc-2.44.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 13:48:34.706246 nso-oc-2.44.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-14 13:48:08.000000 nso-oc-2.44.0/setup.py
```

### Comparing `nso-oc-2.43.2/LICENSE` & `nso-oc-2.44.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/PKG-INFO` & `nso-oc-2.44.0/package_nso_to_oc/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: nso-oc
-Version: 2.43.2
-Summary: Cisco NSO OpenConfig Tools
-Home-page: https://github.com/model-driven-devops/nso-oc-services
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## NSO NED device configuration to OpenConfig
 
 This python package will read in a json configuration for a device and translate to OpenConfig
 
 ### Usage
 1. Decide whether pulling configuration from NSO or reading from file and set the appropriate envars
    - For NSO
@@ -32,8 +24,8 @@
    ```
 3. The below files will be placed in a new directory names "output_data"
    - device_name.json = the full configuration is pulled from NSO
    - device_name_notes.txt = notes resulting from converting NSO config to OpenConfig
    - device_name_openconfig.json = New OpenConfig config
    - device_name_remaining.json = Remaining configuration from NSO
 
-Ideally device_name_openconfig.json + device_name_remaining.json = device_name.json
+Ideally device_name_openconfig.json + device_name_remaining.json = device_name.json
```

### Comparing `nso-oc-2.43.2/README.md` & `nso-oc-2.44.0/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.44.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.43.2
+Version: 2.44.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.43.2/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.44.0/nso_oc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/README.md` & `nso-oc-2.44.0/nso_oc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: nso-oc
+Version: 2.44.0
+Summary: Cisco NSO OpenConfig Tools
+Home-page: https://github.com/model-driven-devops/nso-oc-services
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## NSO NED device configuration to OpenConfig
 
 This python package will read in a json configuration for a device and translate to OpenConfig
 
 ### Usage
 1. Decide whether pulling configuration from NSO or reading from file and set the appropriate envars
    - For NSO
@@ -24,8 +32,8 @@
    ```
 3. The below files will be placed in a new directory names "output_data"
    - device_name.json = the full configuration is pulled from NSO
    - device_name_notes.txt = notes resulting from converting NSO config to OpenConfig
    - device_name_openconfig.json = New OpenConfig config
    - device_name_remaining.json = Remaining configuration from NSO
 
-Ideally device_name_openconfig.json + device_name_remaining.json = device_name.json
+Ideally device_name_openconfig.json + device_name_remaining.json = device_name.json
```

### Comparing `nso-oc-2.43.2/package_nso_to_oc/common.py` & `nso-oc-2.44.0/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/main.py` & `nso-oc-2.44.0/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.44.0/package_nso_to_oc/xe/common_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.44.0/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.44.0/package_nso_to_oc/xe/xe_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.44.0/package_nso_to_oc/xe/xe_bgp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.44.0/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.44.0/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,14 +27,15 @@
             {
                 "openconfig-network-instance:name": "default",
                 "openconfig-network-instance:config": {
                     "openconfig-network-instance:name": "default",
                     "openconfig-network-instance:type": "DEFAULT_INSTANCE",
                     "openconfig-network-instance:enabled": "true"
                 },
+                "openconfig-network-instance:mpls": {"openconfig-network-instance:global": {}},
                 "openconfig-network-instance:protocols": {"openconfig-network-instance:protocol": []},
                 "openconfig-network-instance:interfaces": {"openconfig-network-instance:interface": []},
                 "openconfig-network-instance:vlans": {}
             }
         ]
     }
 }
@@ -91,14 +92,17 @@
             del config_leftover["tailf-ned-cisco-ios:vrf"]["definition"]
         if len(config_leftover["tailf-ned-cisco-ios:vrf"]) == 0:
             del config_leftover["tailf-ned-cisco-ios:vrf"]
     interfaces_by_vrf = get_interfaces_by_vrf(config_before)
     route_forwarding_list_by_vrf = get_route_forwarding_list_by_vrf(config_before)
     configure_network_instances(config_before, config_leftover, interfaces_by_vrf, route_forwarding_list_by_vrf)
 
+    if config_before.get("tailf-ned-cisco-ios:mpls", {}):
+        configure_mpls_default_network_instance(config_before, config_leftover)
+
     if type(config_before.get("tailf-ned-cisco-ios:ip", {}).get("multicast-routing", {}).get("distributed", '')) is list:
         configure_pim_network_instance(config_before, config_leftover)
         configure_igmp_network_instance(config_before, config_leftover)
         configure_cgmp_network_instance(config_before, config_leftover)
 
     cleanup_null_ospf_leftovers(config_leftover)
     cleanup_null_static_route_leftovers(config_leftover)
@@ -307,14 +311,119 @@
         index = 0
         for oc_name in openconfig_network_instances["openconfig-network-instance:network-instances"]["openconfig-network-instance:network-instance"]:
             for oc_instance, oc_instance_name in oc_name.items():
                 if oc_instance_name == instance_name:
                     openconfig_network_instances["openconfig-network-instance:network-instances"]["openconfig-network-instance:network-instance"][index]["openconfig-network-instance:protocols"]["openconfig-network-instance:protocol"].append(network_instance)
             index += 1
 
+def configure_mpls_default_network_instance(config_before, config_leftover):
+
+    """
+    Translates NSO XE NED to MDD OpenConfig Network Instance for MPLS and interface MPLS configuration (default network instance)
+    """
+
+    ttl_propagate = {
+        "openconfig-network-instance:config": {
+            "openconfig-network-instance:ttl-propagation": None
+        }
+    }
+    signaling_protocols = {
+        "openconfig-network-instance:signaling-protocols": {
+            "openconfig-network-instance:ldp": {
+                "openconfig-network-instance:global": {
+                    "openconfig-network-instance:config": {
+                        "openconfig-network-instance:lsr-id": ""
+                    },
+                    "openconfig-network-instance:graceful-restart": {
+                        "openconfig-network-instance:config": {
+                            "openconfig-network-instance:enabled": False
+                        }
+                    }
+                },
+                "openconfig-network-instance:interface-attributes": {
+                    "openconfig-network-instance:config": {
+                        "openconfig-network-instance:hello-holdtime": None,
+                        "openconfig-network-instance:hello-interval": None
+                    }
+                }
+            }
+        }
+    }
+    mpls_interface_attributes = {
+        "openconfig-network-instance:interface-attributes": {
+            "openconfig-network-instance:interface": []
+        }
+    }
+    mpls_interface = {
+        "openconfig-network-instance:interface-id": "",
+        "openconfig-network-instance:config": {
+            "openconfig-network-instance:mpls-enabled": False,
+            "openconfig-network-instance:interface-id": "",
+            "openconfig-network-instance:mpls-mtu": 1500,
+            "openconfig-network-instance:mpls-bgp-forwarding": False
+        },
+        "openconfig-network-instance:interface-ref": {
+            "openconfig-network-instance:config": {
+                "openconfig-network-instance:interface": "",
+                "openconfig-network-instance:subinterface": ""
+            }
+        }
+    }
+
+    propagate_ttl = config_before.get("tailf-ned-cisco-ios:mpls", {}).get("mpls-ip-conf", {}).get("ip", {}).get("propagate-ttl-conf", {}).get("propagate-ttl", {})
+    if propagate_ttl is True:
+        ttl_propagate["openconfig-network-instance:config"]["openconfig-network-instance:ttl-propagation"] = True
+    elif propagate_ttl is False:
+        ttl_propagate["openconfig-network-instance:config"]["openconfig-network-instance:ttl-propagation"] = False
+    openconfig_network_instances["openconfig-network-instance:network-instances"]["openconfig-network-instance:network-instance"][0]["openconfig-network-instance:mpls"]["openconfig-network-instance:global"].update(ttl_propagate)
+    if "mpls-ip-conf" in config_leftover.get("tailf-ned-cisco-ios:mpls", {}):
+        del config_leftover["tailf-ned-cisco-ios:mpls"]["mpls-ip-conf"]
+
+    if config_before.get("tailf-ned-cisco-ios:mpls", {}).get("ldp", {}):
+        if config_before.get("tailf-ned-cisco-ios:mpls", {}).get("ldp", {}).get("graceful-restart-enable", {}).get("graceful-restart", ''):
+            signaling_protocols["openconfig-network-instance:signaling-protocols"]["openconfig-network-instance:ldp"]["openconfig-network-instance:global"]["openconfig-network-instance:graceful-restart"]["openconfig-network-instance:config"]["openconfig-network-instance:enabled"] = True
+        ldp_rid = config_before.get("tailf-ned-cisco-ios:mpls", {}).get("ldp", {}).get("router-id", {}).get("interface", '')
+        if ldp_rid:
+            signaling_protocols["openconfig-network-instance:signaling-protocols"]["openconfig-network-instance:ldp"]["openconfig-network-instance:global"]["openconfig-network-instance:config"]["openconfig-network-instance:lsr-id"] = ldp_rid
+        ldp_disc_holdtime = config_before.get("tailf-ned-cisco-ios:mpls", {}).get("ldp", {}).get("discovery", {}).get("hello", {}).get("holdtime", '')
+        ldp_disc_interval = config_before.get("tailf-ned-cisco-ios:mpls", {}).get("ldp", {}).get("discovery", {}).get("hello", {}).get("interval", '')
+        if ldp_disc_holdtime:
+            signaling_protocols["openconfig-network-instance:signaling-protocols"]["openconfig-network-instance:ldp"]["openconfig-network-instance:interface-attributes"]["openconfig-network-instance:config"]["openconfig-network-instance:hello-holdtime"] = ldp_disc_holdtime
+        if ldp_disc_interval:
+            signaling_protocols["openconfig-network-instance:signaling-protocols"]["openconfig-network-instance:ldp"]["openconfig-network-instance:interface-attributes"]["openconfig-network-instance:config"]["openconfig-network-instance:hello-interval"] = ldp_disc_interval
+        openconfig_network_instances["openconfig-network-instance:network-instances"]["openconfig-network-instance:network-instance"][0]["openconfig-network-instance:mpls"].update(signaling_protocols)
+        del config_leftover["tailf-ned-cisco-ios:mpls"]["ldp"]
+
+    for interface_type in config_before.get("tailf-ned-cisco-ios:interface", {}):
+        for nso_index, value in enumerate(config_before["tailf-ned-cisco-ios:interface"][interface_type]):
+            tmp_mpls_interface = copy.deepcopy(mpls_interface)
+            if value.get("mpls", {}):
+                int_num = str(value['name']).split(".")[0]
+                subint_num = 0
+                if "." in str(value['name']):
+                    subint_num = value['name'].split(".")[1]
+
+                tmp_mpls_interface["openconfig-network-instance:interface-id"] = int_num
+                tmp_mpls_interface["openconfig-network-instance:config"]["openconfig-network-instance:interface-id"] = int_num
+                tmp_mpls_interface["openconfig-network-instance:interface-ref"]["openconfig-network-instance:config"]["openconfig-network-instance:interface"] = interface_type + int_num
+                tmp_mpls_interface["openconfig-network-instance:interface-ref"]["openconfig-network-instance:config"]["openconfig-network-instance:subinterface"] = subint_num
+
+                for mpls_key, mpls_value in value.get("mpls", {}).items():
+                    if "ip" in mpls_key:
+                        tmp_mpls_interface["openconfig-network-instance:config"]["openconfig-network-instance:mpls-enabled"] = True
+                    if "mtu" in mpls_key:
+                        tmp_mpls_interface["openconfig-network-instance:config"]["openconfig-network-instance:mpls-mtu"] = mpls_value
+                    if "bgp" in mpls_key and "forwarding" in mpls_value:
+                        tmp_mpls_interface["openconfig-network-instance:config"]["openconfig-network-instance:mpls-bgp-forwarding"] = True
+
+                mpls_interface_attributes["openconfig-network-instance:interface-attributes"]["openconfig-network-instance:interface"].append(tmp_mpls_interface)
+                del config_leftover["tailf-ned-cisco-ios:interface"][interface_type][nso_index]["mpls"]
+
+    openconfig_network_instances["openconfig-network-instance:network-instances"]["openconfig-network-instance:network-instance"][0]["openconfig-network-instance:mpls"]["openconfig-network-instance:global"].update(mpls_interface_attributes)
+    del config_leftover["tailf-ned-cisco-ios:mpls"]
 
 def configure_igmp_network_instance(config_before, config_leftover):
     """
     Translates NSO XE NED to MDD OpenConfig Network Instance for IP multicast and interface IGMP configuration
     """
 
     igmp_protocol_by_networkinstance = {}
```

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.44.0/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.44.0/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.44.0/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.44.0/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.44.0/package_nso_to_oc/xe/xe_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.44.0/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.44.0/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.44.0/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.44.0/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.44.0/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.44.0/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.2/setup.py` & `nso-oc-2.44.0/setup.py`

 * *Files identical despite different names*

