# Comparing `tmp/shieldcloudapi-0.1.3.tar.gz` & `tmp/shieldcloudapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shieldcloudapi-0.1.3.tar", last modified: Tue Mar 21 03:53:46 2023, max compression
+gzip compressed data, was "shieldcloudapi-0.1.4.tar", last modified: Fri Apr 14 01:49:48 2023, max compression
```

## Comparing `shieldcloudapi-0.1.3.tar` & `shieldcloudapi-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2023-03-21 03:53:46.018430 shieldcloudapi-0.1.3/
--rw-r--r--   0 root         (0) wheel        (0)    11357 2022-09-23 00:22:05.000000 shieldcloudapi-0.1.3/LICENSE
--rw-r--r--   0 root         (0) wheel        (0)    13856 2023-03-21 03:53:46.018250 shieldcloudapi-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) wheel        (0)      319 2022-10-06 06:39:17.000000 shieldcloudapi-0.1.3/README.md
--rw-r--r--   0 root         (0) wheel        (0)      643 2023-03-21 03:37:46.000000 shieldcloudapi-0.1.3/pyproject.toml
--rw-r--r--   0 root         (0) wheel        (0)       38 2023-03-21 03:53:46.018472 shieldcloudapi-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) wheel        (0)      339 2023-03-21 03:40:14.000000 shieldcloudapi-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2023-03-21 03:53:46.017421 shieldcloudapi-0.1.3/shieldcloudapi/
--rw-r--r--   0 root         (0) wheel        (0)        0 2022-09-23 00:25:48.000000 shieldcloudapi-0.1.3/shieldcloudapi/__init__.py
--rw-r--r--   0 root         (0) wheel        (0)    17318 2023-03-21 03:34:28.000000 shieldcloudapi-0.1.3/shieldcloudapi/shieldcloudapi.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2023-03-21 03:53:46.018048 shieldcloudapi-0.1.3/shieldcloudapi.egg-info/
--rw-r--r--   0 root         (0) wheel        (0)    13856 2023-03-21 03:53:46.000000 shieldcloudapi-0.1.3/shieldcloudapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) wheel        (0)      253 2023-03-21 03:53:46.000000 shieldcloudapi-0.1.3/shieldcloudapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) wheel        (0)        1 2023-03-21 03:53:46.000000 shieldcloudapi-0.1.3/shieldcloudapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) wheel        (0)       15 2023-03-21 03:53:46.000000 shieldcloudapi-0.1.3/shieldcloudapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2023-04-14 01:49:48.437787 shieldcloudapi-0.1.4/
+-rw-r--r--   0 root         (0) wheel        (0)    11357 2022-09-23 00:22:05.000000 shieldcloudapi-0.1.4/LICENSE
+-rw-r--r--   0 root         (0) wheel        (0)    13856 2023-04-14 01:49:48.437598 shieldcloudapi-0.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) wheel        (0)      319 2022-10-06 06:39:17.000000 shieldcloudapi-0.1.4/README.md
+-rw-r--r--   0 root         (0) wheel        (0)      643 2023-04-14 01:48:00.000000 shieldcloudapi-0.1.4/pyproject.toml
+-rw-r--r--   0 root         (0) wheel        (0)       38 2023-04-14 01:49:48.437831 shieldcloudapi-0.1.4/setup.cfg
+-rw-r--r--   0 root         (0) wheel        (0)      339 2023-03-21 03:40:14.000000 shieldcloudapi-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2023-04-14 01:49:48.436813 shieldcloudapi-0.1.4/shieldcloudapi/
+-rw-r--r--   0 root         (0) wheel        (0)        0 2022-09-23 00:25:48.000000 shieldcloudapi-0.1.4/shieldcloudapi/__init__.py
+-rw-r--r--   0 root         (0) wheel        (0)    20502 2023-04-14 01:47:28.000000 shieldcloudapi-0.1.4/shieldcloudapi/shieldcloudapi.py
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2023-04-14 01:49:48.437405 shieldcloudapi-0.1.4/shieldcloudapi.egg-info/
+-rw-r--r--   0 root         (0) wheel        (0)    13856 2023-04-14 01:49:48.000000 shieldcloudapi-0.1.4/shieldcloudapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) wheel        (0)      253 2023-04-14 01:49:48.000000 shieldcloudapi-0.1.4/shieldcloudapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) wheel        (0)        1 2023-04-14 01:49:48.000000 shieldcloudapi-0.1.4/shieldcloudapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) wheel        (0)       15 2023-04-14 01:49:48.000000 shieldcloudapi-0.1.4/shieldcloudapi.egg-info/top_level.txt
```

### Comparing `shieldcloudapi-0.1.3/LICENSE` & `shieldcloudapi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shieldcloudapi-0.1.3/PKG-INFO` & `shieldcloudapi-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shieldcloudapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Intrusion Inc Shield Cloud API package
 Author: John Edwards
 Author-email: John Edwards <john.edwards@intrusion.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `shieldcloudapi-0.1.3/pyproject.toml` & `shieldcloudapi-0.1.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "shieldcloudapi"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="John Edwards", email="john.edwards@intrusion.com" },
 ]
 description = "Intrusion Inc Shield Cloud API package"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `shieldcloudapi-0.1.3/shieldcloudapi/shieldcloudapi.py` & `shieldcloudapi-0.1.4/shieldcloudapi/shieldcloudapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import dns.rdataclass
 import dns.rdatatype
 import dns.query
 
 import os
 import copy
 
+import socket
+
 # the following commented out code belongs in the shieldmethod class
 
 # methods that are called before DNS resolution (effectively replacing it) are in this list:
 # PRE_RESOLVE_METHODS = [SHIELD_CLOUD_API_V1, SHIELD_DNS_API_JSON, GOOGLE_DOH]
 
 # methods that are called after DNS resolution are in this list:
 # POST_RESOLVE_METHODS = [
@@ -253,14 +255,19 @@
         #dns_default = ["198.58.73.39"]
         dns_default = ["131.186.6.89"]
 
         if not dns_hosts:
             dns_hosts = dns_default
 
         session["dnshosts"] = dns_hosts
+        
+        # these things should come from config hash
+        session["timeout"] = 3
+        session["maxretries"] = 3   # maximum number of retries across all hosts
+
 
         # use apikey as a substitute for the auth product
         if not apikey:
             apikey = apikeyfile()
 
         if not apikey:
             raise ValueError("init: invalid auth product")
@@ -474,17 +481,45 @@
 
     # validate that it made a query?
     # print("DEBUG 1")
     # print(q.to_text())
 
     # print("DNS: " + dns_server)
 
-    # run the query
-    # implement timeout here later
-    (r, tcp) = dns.query.udp_with_fallback(q, dns_server)
+    maxretries = 3 # change to session variable
+    retries = 0
+    answer = False
+    
+
+    while retries < maxretries and not answer:
+        retries = retries + 1
+        # run the query
+        # implement timeout here later
+
+        # change the server according to the load balance algo before each run
+
+        # set a timer here
+        try:
+            (r, tcp) = dns.query.udp_with_fallback(q, dns_server)
+            if not r.answer:
+                print("No answer from {} to attempt {}".format(dns_server,retries))
+                print("Query: {}".format(q))
+
+                print("Session: {}".format(session))
+            else:
+                answer = True
+
+
+        except dns.exception.Timeout:
+            print("DNS Timeout")
+        except Exception as e:
+            print("DNS Exception: {}".format(e))
+
+    if not answer:
+        return False
 
     # use doh_simple code from lambda to turn the wirecode response into a python object
     # print("DEBUG 2")
     # print(r.to_text())
 
     p = to_doh_simple(r)
 
@@ -520,14 +555,101 @@
 
     # need to test for failure here in case session["method"] is not valid
 
     #print("=== end query_dns ===")
     return result
 
 
+def valid_ip(ipaddr):
+    try:
+        socket.inet_aton(ipaddr)
+        return 4
+    except socket.error:
+        return False
+
+def query_ip(session,ipaddr,verbose=False):
+    block = False
+    allow = False
+
+    #check if it is a valid ipv4 or ipv6 address
+
+    ipversion = valid_ip(ipaddr)
+    if not ipversion:
+        return False
+    elif ipversion == 4:
+        fqdn = "{}.ip.shield-cloud.com".format(ipaddr)
+        result = query_dns(session,fqdn)
+
+        if "Answer" in result and "data" in result["Answer"][0]:
+            #print(result["Answer"][0]["data"])
+            if result["Answer"][0]["data"].startswith("127"):
+                block = True
+                allow = False
+            else:
+                block = False
+                allow = True
+
+            if verbose:
+                # use element 0 in case we one day want to return multiple answers
+                result["Answer"][0]["Block"] = block
+                result["Answer"][0]["Allow"] = allow
+                return result
+
+            elif block:
+                return "BLOCK"
+            elif allow:
+                return "ALLOW"
+            else:
+                return False
+        
+        # provide data if it didn't come back with an answer
+        if verbose:
+            return result
+        else:
+            return False
+
+    print("ipversion was {}".format(ipversion))
+
+# this function returns 2 items if successful
+#   a netmask in CIDR format
+#   an action (ie: block or deny)
+def query_netmask(session,ipaddr):
+
+    ret = {}
+
+    result = query_ip(session,ipaddr,True)
+    if not result:
+        print("NOT RESULT")
+        return False
+   
+
+    print("Block: {}".format(result["Answer"][0]["Block"]))
+
+    if result["Answer"][0]["Block"] == True:
+        ret["Action"] = "BLOCK"
+        if "Additional" in result:
+            # process reply to add whole netmask
+            #ret["Netmask"] = "not done yet"
+
+            ret["NetMask"] = "{}/32".format(ipaddr)
+
+        else:
+            ret["NetMask"] = "{}/32".format(ipaddr)
+
+    elif result["Answer"][0]["Allow"] == True:
+        ret["Action"] = "ALLOW"
+        ret["NetMask"] = "{}/32".format(ipaddr)
+    else:
+        print("ELSE")
+        return result
+
+
+    return ret
+
+
 def query(session, domain, querytype="ANY"):
     # basic host request
     # return block or allow
     # return list of blocked IP addresses
     # return list of allowed IP addresses
 
     return false
```

### Comparing `shieldcloudapi-0.1.3/shieldcloudapi.egg-info/PKG-INFO` & `shieldcloudapi-0.1.4/shieldcloudapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shieldcloudapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Intrusion Inc Shield Cloud API package
 Author: John Edwards
 Author-email: John Edwards <john.edwards@intrusion.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

