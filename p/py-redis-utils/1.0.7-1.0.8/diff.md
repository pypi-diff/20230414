# Comparing `tmp/py-redis-utils-1.0.7.tar.gz` & `tmp/py-redis-utils-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-redis-utils-1.0.7.tar", last modified: Thu Apr 13 11:17:15 2023, max compression
+gzip compressed data, was "py-redis-utils-1.0.8.tar", last modified: Fri Apr 14 11:38:37 2023, max compression
```

## Comparing `py-redis-utils-1.0.7.tar` & `py-redis-utils-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-04-13 11:17:15.664458 py-redis-utils-1.0.7/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      414 2023-04-13 11:17:15.664458 py-redis-utils-1.0.7/PKG-INFO
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     1361 2023-04-11 16:05:30.000000 py-redis-utils-1.0.7/README.md
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-04-13 11:17:15.664458 py-redis-utils-1.0.7/py_redis_utils.egg-info/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      414 2023-04-13 11:17:15.000000 py-redis-utils-1.0.7/py_redis_utils.egg-info/PKG-INFO
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      259 2023-04-13 11:17:15.000000 py-redis-utils-1.0.7/py_redis_utils.egg-info/SOURCES.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-04-13 11:17:15.000000 py-redis-utils-1.0.7/py_redis_utils.egg-info/dependency_links.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       21 2023-04-13 11:17:15.000000 py-redis-utils-1.0.7/py_redis_utils.egg-info/requires.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       13 2023-04-13 11:17:15.000000 py-redis-utils-1.0.7/py_redis_utils.egg-info/top_level.txt
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-04-13 11:17:15.664458 py-redis-utils-1.0.7/pyredisutils/
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)       40 2023-04-11 16:05:30.000000 py-redis-utils-1.0.7/pyredisutils/__init__.py
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     6158 2023-04-13 11:13:28.000000 py-redis-utils-1.0.7/pyredisutils/_auth_deco.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-04-13 11:17:15.664458 py-redis-utils-1.0.7/setup.cfg
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)      696 2023-04-13 11:16:56.000000 py-redis-utils-1.0.7/setup.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-04-14 11:38:37.535309 py-redis-utils-1.0.8/
+-rw-r--r--   0 erne      (1000) erne      (1000)      478 2023-04-14 11:38:37.535309 py-redis-utils-1.0.8/PKG-INFO
+-rwxrwxrwx   0 erne      (1000) erne      (1000)     1361 2023-02-03 14:24:27.000000 py-redis-utils-1.0.8/README.md
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-04-14 11:38:37.535309 py-redis-utils-1.0.8/py_redis_utils.egg-info/
+-rw-r--r--   0 erne      (1000) erne      (1000)      478 2023-04-14 11:38:37.000000 py-redis-utils-1.0.8/py_redis_utils.egg-info/PKG-INFO
+-rw-r--r--   0 erne      (1000) erne      (1000)      259 2023-04-14 11:38:37.000000 py-redis-utils-1.0.8/py_redis_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-04-14 11:38:37.000000 py-redis-utils-1.0.8/py_redis_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       21 2023-04-14 11:38:37.000000 py-redis-utils-1.0.8/py_redis_utils.egg-info/requires.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       13 2023-04-14 11:38:37.000000 py-redis-utils-1.0.8/py_redis_utils.egg-info/top_level.txt
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-04-14 11:38:37.535309 py-redis-utils-1.0.8/pyredisutils/
+-rwxrwxrwx   0 erne      (1000) erne      (1000)       39 2023-02-03 12:53:24.000000 py-redis-utils-1.0.8/pyredisutils/__init__.py
+-rw-r--r--   0 erne      (1000) erne      (1000)     6604 2023-04-14 11:37:15.000000 py-redis-utils-1.0.8/pyredisutils/_auth_deco.py
+-rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-04-14 11:38:37.535309 py-redis-utils-1.0.8/setup.cfg
+-rw-r--r--   0 erne      (1000) erne      (1000)      696 2023-04-14 11:37:45.000000 py-redis-utils-1.0.8/setup.py
```

### Comparing `py-redis-utils-1.0.7/README.md` & `py-redis-utils-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `py-redis-utils-1.0.7/pyredisutils/_auth_deco.py` & `py-redis-utils-1.0.8/pyredisutils/_auth_deco.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,56 +36,65 @@
 
             try:
                 logging.info("Connecting to Redis Server")
                 redis_client = redis_instance.client()
                 pubsub = redis_client.pubsub()
                 pubsub.subscribe(channel_name + ".reply")
 
-                publish_message = _transform_dict(publish_message, token, request_id)
-                response_message = _transform_dict(response_message, "", request_id)
+                publish_message = _transform_dict(
+                    publish_message, token, request_id)
+                response_message = _transform_dict(
+                    response_message, "", request_id)
 
-                logging.info("Publishing message to Redis server for token validation.")
+                logging.info(
+                    "Publishing message to Redis server for token validation.")
                 redis_client.publish(
                     channel_name,
                     json.dumps(
                         publish_message
                     ),
                 )
 
                 try:
                     timeout = 5.0
                     live_timeout = time.time() + 5
                     logging.info("Waiting for Redis response.")
-                    pubsub.get_message()
                     while True:
                         if time.time() > live_timeout:
                             raise TimeoutError
                         message = pubsub.get_message(timeout=timeout)
-                        if message:
+                        if message and message["type"] == "message":
                             redis_response = {}
                             for key, value in message.items():
-                                redis_response[key] = _transform_redis_response(value)
-                            diff = deepdiff.DeepDiff(response_message, redis_response)
+                                redis_response[key] = _transform_redis_response(
+                                    value)
+                            diff = deepdiff.DeepDiff(
+                                response_message, redis_response)
                             if diff == {}:
                                 logging.info("Redis response - Token is valid")
                                 break
+                            if "type_changes" in diff:
+                                logging.info(
+                                    "Redis response - Token is invalid")
+                                redis_client.close()
+                                return _make_response("Unauthorized", 401)
                             values = diff.get("values_changed", {})
                             for change in values.values():
-                                if change["old_value"] == request_id:
-                                    continue
-                            logging.info("Redis response - Token is invalid")
-                            return _make_response("Unauthorized", 401)
-                        else:
-                            raise TimeoutError
+                                if change["old_value"] != request_id:
+                                    redis_client.close()
+                                    logging.info(
+                                        "Redis response - Token is invalid")
+                                    return _make_response("Unauthorized", 401)
                 except TimeoutError:
                     logging.error(
                         "Haven't received any answer from Redis for 5 seconds."
                     )
+                    redis_client.close()
                     return _make_response("Gateway Timeout", 504)
-                pubsub.unsubscribe(channel_name + ".reply")
+                redis_client.close()
             except redis.exceptions.ConnectionError:
                 logging.error("Redis refused to connect.")
                 return _make_response("Bad Gateway", 502)
 
             return org_function(*args, **kwargs)
 
         return authorize
```

### Comparing `py-redis-utils-1.0.7/setup.py` & `py-redis-utils-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.0.7"
+VERSION = "1.0.8"
 DESCRIPTION = "Utilities with Redis"
 
 # Setting up
 setup(
     name="py-redis-utils",
     version=VERSION,
     author="KE",
```

