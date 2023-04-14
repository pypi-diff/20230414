# Comparing `tmp/butler-connect-0.4.1.tar.gz` & `tmp/butler-connect-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butler-connect-0.4.1.tar", last modified: Tue Apr 11 15:46:23 2023, max compression
+gzip compressed data, was "butler-connect-0.4.2.tar", last modified: Fri Apr 14 13:25:16 2023, max compression
```

## Comparing `butler-connect-0.4.1.tar` & `butler-connect-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 15:46:23.276066 butler-connect-0.4.1/
--rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     1886 2023-04-11 15:46:23.275067 butler-connect-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      135 2023-03-22 08:42:33.000000 butler-connect-0.4.1/README.md
--rw-rw-rw-   0        0        0      738 2023-04-11 15:45:57.000000 butler-connect-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 15:46:23.276066 butler-connect-0.4.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 15:46:23.252828 butler-connect-0.4.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 15:46:23.255827 butler-connect-0.4.1/src/butlerConnect/
--rw-rw-rw-   0        0        0       43 2022-12-30 14:11:10.000000 butler-connect-0.4.1/src/butlerConnect/__init__.py
--rw-rw-rw-   0        0        0    16289 2023-03-22 08:41:04.000000 butler-connect-0.4.1/src/butlerConnect/pikaButler.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:46:23.258827 butler-connect-0.4.1/src/butlerDescription/
--rw-rw-rw-   0        0        0      108 2022-12-30 15:11:11.000000 butler-connect-0.4.1/src/butlerDescription/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.4.1/src/butlerDescription/component.py
--rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.4.1/src/butlerDescription/control.py
--rw-rw-rw-   0        0        0     1570 2023-01-18 19:27:38.000000 butler-connect-0.4.1/src/butlerDescription/signal.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:46:23.274068 butler-connect-0.4.1/src/butler_connect.egg-info/
--rw-rw-rw-   0        0        0     1886 2023-04-11 15:46:23.000000 butler-connect-0.4.1/src/butler_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-04-11 15:46:23.000000 butler-connect-0.4.1/src/butler_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 15:46:23.000000 butler-connect-0.4.1/src/butler_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-04-11 15:46:23.000000 butler-connect-0.4.1/src/butler_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-04-11 15:46:23.000000 butler-connect-0.4.1/src/butler_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 13:25:16.796179 butler-connect-0.4.2/
+-rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0     1886 2023-04-14 13:25:16.795183 butler-connect-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0      135 2023-03-22 08:42:33.000000 butler-connect-0.4.2/README.md
+-rw-rw-rw-   0        0        0      738 2023-04-14 13:24:45.000000 butler-connect-0.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:25:16.796179 butler-connect-0.4.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 13:25:16.726553 butler-connect-0.4.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 13:25:16.754663 butler-connect-0.4.2/src/butlerConnect/
+-rw-rw-rw-   0        0        0       43 2022-12-30 14:11:10.000000 butler-connect-0.4.2/src/butlerConnect/__init__.py
+-rw-rw-rw-   0        0        0    16359 2023-04-14 13:24:24.000000 butler-connect-0.4.2/src/butlerConnect/pikaButler.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:25:16.762175 butler-connect-0.4.2/src/butlerDescription/
+-rw-rw-rw-   0        0        0      108 2022-12-30 15:11:11.000000 butler-connect-0.4.2/src/butlerDescription/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.4.2/src/butlerDescription/component.py
+-rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.4.2/src/butlerDescription/control.py
+-rw-rw-rw-   0        0        0     1570 2023-01-18 19:27:38.000000 butler-connect-0.4.2/src/butlerDescription/signal.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:25:16.794180 butler-connect-0.4.2/src/butler_connect.egg-info/
+-rw-rw-rw-   0        0        0     1886 2023-04-14 13:25:16.000000 butler-connect-0.4.2/src/butler_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-04-14 13:25:16.000000 butler-connect-0.4.2/src/butler_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:25:16.000000 butler-connect-0.4.2/src/butler_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-04-14 13:25:16.000000 butler-connect-0.4.2/src/butler_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-14 13:25:16.000000 butler-connect-0.4.2/src/butler_connect.egg-info/top_level.txt
```

### Comparing `butler-connect-0.4.1/LICENSE` & `butler-connect-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `butler-connect-0.4.1/PKG-INFO` & `butler-connect-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.4.1
+Version: 0.4.2
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `butler-connect-0.4.1/pyproject.toml` & `butler-connect-0.4.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "butler-connect"
-version = "0.4.1"
+version = "0.4.2"
 description = "Access libraries (with pika) and data definitions for the Buttler project."
 readme = "README.md"
 authors = [{ name = "Oliver Birkholz", email = "info@aibutler.de" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `butler-connect-0.4.1/src/butlerConnect/pikaButler.py` & `butler-connect-0.4.2/src/butlerConnect/pikaButler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 
 import pika, logging, time, os
 from pika import frame
 from pika.exchange_type import ExchangeType
 
+from pika.exceptions import *
+
 LOG = logging.getLogger(__name__)
 import queue
 import threading
 
 import ssl
 
 default_heartbeat = 600
@@ -183,24 +185,20 @@
     def stop(self):
         self.isRunning = False
     
     def thread(self):
         while self.isRunning :
             try:
                 self.run()
-
+            except (ConnectionResetError, StreamLostError ) as e:
+                LOG.warning(f'Loosing connection. Do a reset!')
             except Exception as e:
                 if self.isRunning:
                     desc = f'Exception Connection from {self.topic}@{self.connectionParameter}'
                     LOG.exception(desc)
-            '''
-            except (pika.exceptions.IncompatibleProtocolError, pika.exceptions.StreamLostError):
-                desc = f'Loosing Connection from {self.topic}@{self.connectionParameter}'
-                LOG.warning(desc)
-            '''
             if self.isRunning:
                 time.sleep(self.reconnectingTimeout )
                 LOG.info(f'Try to reconnect!')
     
     def run(self):
         pass
 
@@ -256,23 +254,27 @@
         
         while self.isRunning :
             try:
                 item = self.que.get(block=True,timeout=default_heartbeat/2)
             except:
                 item = {}      
             if item != {}:
-                for topic in item.keys():
-                    d = item[topic]
-                    msg = d.get('msg')
-                    routing_key = d.get('routing_key',None)
-                    if routing_key == None: routing_key = ''
-                    LOG.info(f'publish data {topic}@{msg}')
-                    self.channel.basic_publish(exchange=topic,
-                            routing_key=routing_key,
-                            body=msg)
+                try:
+                    for topic in item.keys():
+                        d = item[topic]
+                        msg = d.get('msg')
+                        routing_key = d.get('routing_key',None)
+                        if routing_key == None: routing_key = ''
+                        LOG.info(f'publish data {topic}@{msg}')
+                        self.channel.basic_publish(exchange=topic,
+                                routing_key=routing_key,
+                                body=msg)
+                except Exception as e:
+                    self.que.put(item)
+                    raise e
                 self.que.task_done()
 
             
     def publish(self,topic,msg,routing_key=None):
         LOG.info(f'publish {topic}=>{msg} with routing_key={routing_key}')
         self.que.put_nowait({topic:{'msg':msg,'routing_key':routing_key}})
     def stop(self):
```

### Comparing `butler-connect-0.4.1/src/butlerDescription/control.py` & `butler-connect-0.4.2/src/butlerDescription/control.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.4.1/src/butlerDescription/signal.py` & `butler-connect-0.4.2/src/butlerDescription/signal.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.4.1/src/butler_connect.egg-info/PKG-INFO` & `butler-connect-0.4.2/src/butler_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.4.1
+Version: 0.4.2
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

