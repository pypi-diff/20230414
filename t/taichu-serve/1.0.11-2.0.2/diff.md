# Comparing `tmp/taichu-serve-1.0.11.tar.gz` & `tmp/taichu-serve-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-serve-1.0.11.tar", last modified: Tue Apr 11 08:59:04 2023, max compression
+gzip compressed data, was "taichu-serve-2.0.2.tar", last modified: Fri Apr 14 06:11:49 2023, max compression
```

## Comparing `taichu-serve-1.0.11.tar` & `taichu-serve-2.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 08:59:04.811370 taichu-serve-1.0.11/
--rw-r--r--   0 chen       (501) staff       (20)      236 2023-04-11 08:59:04.811127 taichu-serve-1.0.11/PKG-INFO
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 08:59:04.809610 taichu-serve-1.0.11/model_service/
--rw-r--r--   0 chen       (501) staff       (20)      188 2023-02-07 00:50:51.000000 taichu-serve-1.0.11/model_service/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     8308 2023-04-10 07:48:58.000000 taichu-serve-1.0.11/model_service/app.py
--rw-r--r--   0 chen       (501) staff       (20)     1302 2023-04-10 07:48:58.000000 taichu-serve-1.0.11/model_service/command.py
--rw-r--r--   0 chen       (501) staff       (20)      935 2023-04-03 11:34:16.000000 taichu-serve-1.0.11/model_service/common.py
--rw-r--r--   0 chen       (501) staff       (20)     1290 2023-04-03 11:12:47.000000 taichu-serve-1.0.11/model_service/error_code.py
--rw-r--r--   0 chen       (501) staff       (20)     6391 2023-04-03 09:59:12.000000 taichu-serve-1.0.11/model_service/grpc_predict_v2_pb2.py
--rw-r--r--   0 chen       (501) staff       (20)    12997 2023-04-03 09:59:12.000000 taichu-serve-1.0.11/model_service/grpc_predict_v2_pb2_grpc.py
--rw-r--r--   0 chen       (501) staff       (20)     3572 2023-04-11 04:36:47.000000 taichu-serve-1.0.11/model_service/grpc_server.py
--rw-r--r--   0 chen       (501) staff       (20)     2090 2023-04-03 11:30:51.000000 taichu-serve-1.0.11/model_service/log.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 08:59:04.809947 taichu-serve-1.0.11/model_service/model_def/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-02-07 00:50:51.000000 taichu-serve-1.0.11/model_service/model_def/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     1761 2023-02-07 00:50:51.000000 taichu-serve-1.0.11/model_service/model_def/model_def.py
--rw-r--r--   0 chen       (501) staff       (20)     5225 2023-04-03 06:17:46.000000 taichu-serve-1.0.11/model_service/model_service.py
--rw-r--r--   0 chen       (501) staff       (20)     1061 2023-04-10 07:48:58.000000 taichu-serve-1.0.11/model_service/settings.py
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-11 08:59:04.811428 taichu-serve-1.0.11/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      952 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/setup.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 08:59:04.810922 taichu-serve-1.0.11/taichu_serve.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      236 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      609 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       74 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/entry_points.txt
--rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)       14 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/top_level.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-14 06:11:49.152250 taichu-serve-2.0.2/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-14 06:11:49.152112 taichu-serve-2.0.2/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-14 06:11:49.152290 taichu-serve-2.0.2/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      949 2023-04-14 06:11:45.000000 taichu-serve-2.0.2/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-14 06:11:49.150879 taichu-serve-2.0.2/taichu_serve/
+-rw-r--r--   0 chen       (501) staff       (20)     3398 2023-04-14 02:56:12.000000 taichu-serve-2.0.2/taichu_serve/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     9214 2023-04-14 05:19:23.000000 taichu-serve-2.0.2/taichu_serve/app.py
+-rw-r--r--   0 chen       (501) staff       (20)     2410 2023-04-14 05:13:39.000000 taichu-serve-2.0.2/taichu_serve/command.py
+-rw-r--r--   0 chen       (501) staff       (20)      948 2023-04-13 09:06:46.000000 taichu-serve-2.0.2/taichu_serve/common.py
+-rw-r--r--   0 chen       (501) staff       (20)     1521 2023-04-14 04:52:00.000000 taichu-serve-2.0.2/taichu_serve/error_code.py
+-rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.2/taichu_serve/grpc_predict_v2_pb2.py
+-rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.2/taichu_serve/grpc_predict_v2_pb2_grpc.py
+-rw-r--r--   0 chen       (501) staff       (20)     3572 2023-04-14 05:10:28.000000 taichu-serve-2.0.2/taichu_serve/grpc_server.py
+-rw-r--r--   0 chen       (501) staff       (20)     2103 2023-04-13 09:06:46.000000 taichu-serve-2.0.2/taichu_serve/log.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-14 06:11:49.151939 taichu-serve-2.0.2/taichu_serve/model_def/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-02-07 00:50:51.000000 taichu-serve-2.0.2/taichu_serve/model_def/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     5444 2023-04-14 01:39:52.000000 taichu-serve-2.0.2/taichu_serve/model_server.py
+-rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.2/taichu_serve/ratelimiter.py
+-rw-r--r--   0 chen       (501) staff       (20)     1924 2023-04-14 05:14:20.000000 taichu-serve-2.0.2/taichu_serve/settings.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-14 06:11:49.151798 taichu-serve-2.0.2/taichu_serve.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-14 06:11:49.000000 taichu-serve-2.0.2/taichu_serve.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      587 2023-04-14 06:11:49.000000 taichu-serve-2.0.2/taichu_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-14 06:11:49.000000 taichu-serve-2.0.2/taichu_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       73 2023-04-14 06:11:49.000000 taichu-serve-2.0.2/taichu_serve.egg-info/entry_points.txt
+-rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-14 06:11:49.000000 taichu-serve-2.0.2/taichu_serve.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-14 06:11:49.000000 taichu-serve-2.0.2/taichu_serve.egg-info/top_level.txt
```

### Comparing `taichu-serve-1.0.11/model_service/app.py` & `taichu-serve-2.0.2/taichu_serve/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,102 +1,190 @@
 # -*- coding: utf-8 -*-
 """
 DL webservice app
 """
+import ctypes
 import inspect
 import json
 import logging
 import os
 import threading
 import time
 import traceback
 import uuid
 
 from flask import Flask, request, g
 
-import log
-from settings import parse_args
+from taichu_serve.log import init_logger
+from taichu_serve.settings import parse_args
+from taichu_serve.ratelimiter import semaphore
 
-log.init_logger()
+init_logger()
 
 app = Flask("aa")
 
-from error_code import ModelNotFoundError, ModelPredictError
+from taichu_serve.error_code import ModelNotFoundError, ModelPredictError, TooManyRequestsError
+from taichu_serve import Service
+from taichu_serve.common import Local
 
 LOGGER = logging.getLogger(__name__)
-import argparse
 
-from model_service.model_service import SingleNodeService
+import multiprocessing
 
+args = parse_args()
 
-def init_model_service_instance():
+workers_status = []
+
+
+class WorkersPipeMgr(object):
+    def __init__(self, num):
+        self._list = []
+        self._occupied = []
+        self._lock = threading.Lock()
+        self._num = num
+
+    def append(self, pipe):
+        with self._lock:
+            self._list.append(pipe)
+            self._occupied.append(False)
+
+    def acquire(self, request_id):
+        with self._lock:
+            hash_value = hash(request_id)
+            index = hash_value % self._num
+
+            if not self._occupied[index]:
+                self._occupied[index] = True
+                return self._list[index]
+
+            return None
+
+    def release(self, request_id):
+        with self._lock:
+            hash_value = hash(request_id)
+            index = hash_value % self._num
+
+            if self._occupied[index]:
+                self._occupied[index] = False
+
+
+workers_pipe = WorkersPipeMgr(args.instances_num)
+
+
+def worker_main_loop(args, pipe, status):
     # pwd = os.path.dirname(os.path.abspath(__file__))
 
-    args = parse_args()
+    # args = parse_args()
 
     LOGGER.info("args: %s", args)
 
-    from model_service.model_service import load_service
+    from taichu_serve.model_server import load_service
     dict_model_service = {}
 
     model_path = os.path.abspath(args.model_path)
     # model_name = args.model_name
 
     model_service_file = args.service_file
 
     print(
         "model_path={} \n model_service_file={} "
         .format(model_path, model_service_file))
 
     module = load_service(os.path.join(model_path, model_service_file)
-                          ) if model_service_file else SingleNodeService
+                          ) if model_service_file else Service
     classes = [cls[1] for cls in inspect.getmembers(module, inspect.isclass)]
 
-    # assert len(classes) >= 1, \
-    #     'No valid python class derived from Base Model Service is in module file: %s' % \
-    #     model_service_file
+    assert len(classes) > 0, "There should be one user defined service derived from ModelService."
 
     class_defs = list(
         filter(
-            lambda c: issubclass(c, SingleNodeService) and len(
+            lambda c: issubclass(c, Service) and len(
                 c.__subclasses__()) == 0, classes))
 
     # if len(class_defs) != 1:
     #     raise Exception(
     #         'There should be one user defined service derived from ModelService.'
     #     )
+    assert len(class_defs) > 0, "There should be one user defined service derived from ModelService."
 
     for c in class_defs:
         LOGGER.info("class_defs: %s", c.__name__)
         instance = c(model_path)
-        threading.Thread(target=instance.warmup).start()
+        # threading.Thread(target=instance.warmup).start()
+        instance.warmup()
         dict_model_service[f'{str(c.__name__).lower()}_{instance.model_version.lower()}'] = instance
 
     # model_service = class_defs[0](model_path)
+    status.value = 0
+    LOGGER.info("model service init done")
+
+    while True:
+        data = pipe.recv()
+        try:
+            model_name = data.get('model_name')
+            model_version = data.get('model_version')
+            request_id = data.get('request_id', str(uuid.uuid4()))
+
+            Local.request_id = request_id
+            ins = dict_model_service.get(f'{model_name.lower()}_{model_version.lower()}', None)
+            if ins is None:
+                ret = {
+                    'data': None,
+                    'status': 'error',
+                    'error': 'model not found',
+                }
+            else:
+                ret = {
+                    'data': ins.inference(data.get('data'), request_id),
+                    'status': 'ok',
+                }
+        except Exception as e:
+            LOGGER.error(traceback.format_exc())
+            ret = {
+                'data': None,
+                'status': 'error',
+                'error': str(e),
+            }
+        pipe.send(ret)
 
-    return dict_model_service
+    # return dict_model_service
 
 
-model_service = init_model_service_instance()
+def model_inference(model_name, model_version, data, request_id):
+    try:
+        p = workers_pipe.acquire(request_id)
+        if p is None:
+            raise TooManyRequestsError()
+        p.send({'model_name': model_name, 'model_version': model_version, 'data': data, 'request_id': request_id})
+        ret = p.recv()
+
+        if ret.get('status') == 'error':
+            raise ModelPredictError(message=ret.get('error'))
+        return ret.get('data')
+    finally:
+        if p is not None:
+            workers_pipe.release(request_id)
 
 
-def get_model_service(model_name, model_version):
-    model_name = model_name.lower()
-    model_version = model_version.lower()
-    ins = model_service.get(f'{model_name}_{model_version}', None)
-    if ins is None:
-        raise ModelNotFoundError(message=f'Model {model_name} version {model_version} not found')
-    return ins
+def init_model_service_instance():
+    for i in range(args.instances_num):
+        p1, p2 = multiprocessing.Pipe()
+        status = multiprocessing.Value('i', -1)
+        workers_status.append(status)
+        LOGGER.info("start worker %s", i)
+        multiprocessing.Process(target=worker_main_loop, args=(args, p2, status)
+                                ).start()
+        workers_pipe.append(p1)
 
 
 def is_all_model_ready():
-    if len(model_service) == 0:
+    if len(workers_status) != args.instances_num:
         return False
-    for k, instance in model_service.items():
-        if not instance.ready:
+    for stat in workers_status:
+        if stat.value != 0:
             return False
 
     return True
 
 
 @app.before_request
 def add_request_id():
@@ -115,16 +203,31 @@
         else:
             request_id = str(uuid.uuid4())
         setattr(g, 'request_id', request_id)
     except Exception as e:
         logging.error(str(e))
 
 
+@app.before_request
+def limiter():
+    if request.path == '/health/live' or request.path == '/health/ready':
+        return
+
+    ok = semaphore.acquire(blocking=False)
+    LOGGER.info('semaphore.acquire:{}'.format(ok))
+    g.is_limited = not ok
+    if not ok:
+        return {'error': '请求过于频繁，请稍后再试'}, 429, {'Content-Type': 'application/json'}
+
+
 @app.after_request
 def after_request(response):
+    if hasattr(g, 'is_limited') and not g.is_limited:
+        semaphore.release()
+
     try:
         extra = {
             # 'id': str(uuid.uuid4()),
             'http_method': request.method,
             'endpoint': request.endpoint,
             'url_path': request.path,
             'url_query': request.query_string.decode('utf-8'),
@@ -175,108 +278,33 @@
     ret = {
         'id': request_id,
         'model_name': model_name,
         'model_version': model_version,
         'parameters': {}
     }
 
-    instance = get_model_service(model_name, model_version)
+    # instance = get_model_service(model_name, model_version)
 
     try:
-        res = instance.inference(req.get('parameters', {}), context={})
+        res = model_inference(model_name, model_version, req.get('parameters', {}), request_id)
+    except TooManyRequestsError as e:
+        LOGGER.info('Too many requests!')
+        return {'error': '请求过于频繁，请稍后再试'}, 429, {'Content-Type': 'application/json'}
     except Exception as e:
         LOGGER.error('Algorithm crashed!')
         LOGGER.error(traceback.format_exc())
         raise ModelPredictError(message=str(e))
 
     ret['parameters'] = res
     return json.dumps(ret, ensure_ascii=False), 200, {
         'Content-Type': 'application/json'
     }
 
 
-# @app.route('/', methods=['POST'])
-# def inference_task():
-#     # get all data from different media
-#     rec_dict = {}
-#
-#     def parse_file(f):
-#         if isinstance(f.stream, tempfile.SpooledTemporaryFile):
-#             return f.filename, io.BytesIO(f.stream.read())
-#         elif isinstance(one.stream, io.BytesIO):
-#             return f.filename, f.stream
-#         else:
-#             LOGGER.error('receive file not recognized!')
-#             raise Exception
-#
-#     if request.form or request.files:
-#         form = request.form
-#         files = request.files
-#         rec_dict = {}
-#         for k, v in form.items():
-#             rec_dict[k] = v
-#
-#         for k, file in files.items():
-#             lst = files.getlist(k)
-#             if len(lst) == 1:
-#                 one = lst[0]
-#                 filename, file_content = parse_file(one)
-#                 rec_dict[k] = (filename, file_content)
-#
-#                 continue
-#
-#             filename_dict = collections.OrderedDict()
-#             for one in lst:
-#                 filename, file_content = parse_file(one)
-#                 filename_dict[filename] = file_content
-#
-#             rec_dict[k] = filename_dict
-#     elif request.json:
-#
-#         rec_dict = request.json
-#     else:
-#         return get_result_json(MR0101()), 400, {
-#             'Content-Type': 'application/json'
-#         }
-#
-#     args = request.args
-#     for k, v in args.items():
-#         rec_dict[k] = v
-#
-#     try:
-#         res = model_service.inference(rec_dict)
-#         return json.dumps(res, ensure_ascii=False), 200, {
-#             'Content-Type': 'application/json'
-#         }
-#     except KeyError as k:
-#         LOGGER.error('Algorithm crashed!')
-#         LOGGER.error(traceback.format_exc())
-#         return get_result_json(MR0105()), 400, {
-#             'Content-Type': 'application/json'
-#         }
-#     except TypeError as te:
-#         LOGGER.error('Algorithm crashed!')
-#         LOGGER.error(traceback.format_exc())
-#         return get_result_json(MR0105()), 400, {
-#             'Content-Type': 'application/json'
-#         }
-#     except Exception as e:
-#         LOGGER.error('Algorithm crashed!')
-#         LOGGER.error(traceback.format_exc())
-#         return get_result_json(MR0105()), 500, {
-#             'Content-Type': 'application/json'
-#         }
-
-
 def get_result_json(ais_error):
     """
         Create a json response with error code and error message
     """
     data = ais_error.to_dict()
     data['words_result'] = {}
 
     return json.dumps(data, ensure_ascii=False)
-
-# if __name__ == "__main__":
-#     args = parser.parse_args()
-# else:
-#     args = parser.parse_args(os.environ['TF_MODEL_ARGS'].split())
```

### Comparing `taichu-serve-1.0.11/model_service/common.py` & `taichu-serve-2.0.2/taichu_serve/common.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import threading
 import time
 import uuid
 
 import grpc
 
-from error_code import ModelPredictError, ModelNotFoundError
+from taichu_serve.error_code import ModelPredictError, ModelNotFoundError
 
 Local = threading.local()
 logger = logging.getLogger(__name__)
 
 
 def grpc_interceptor(func):
     @functools.wraps(func)
```

### Comparing `taichu-serve-1.0.11/model_service/error_code.py` & `taichu-serve-2.0.2/taichu_serve/error_code.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,14 +31,23 @@
         self.code = code
         self.message = message
 
     def __str__(self):
         return self.message
 
 
+class TooManyRequestsError(Exception):
+    def __init__(self, code='TooManyRequestsError', message='Too many requests'):
+        self.code = code
+        self.message = message
+
+    def __str__(self):
+        return self.message
+
+
 class MR0100(ModelArtsError):
     'Specific ModelArts error'
     code = 'MR.0100'
     msg = 'Succeeded'
 
 
 class MR0101(ModelArtsError):
```

### Comparing `taichu-serve-1.0.11/model_service/grpc_predict_v2_pb2.py` & `taichu-serve-2.0.2/taichu_serve/grpc_predict_v2_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15grpc_predict_v2.proto\x12\x0ctaichu_infer\"\x13\n\x11ServerLiveRequest\"\"\n\x12ServerLiveResponse\x12\x0c\n\x04live\x18\x01 \x01(\x08\"\x14\n\x12ServerReadyRequest\"$\n\x13ServerReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\"2\n\x11ModelReadyRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"#\n\x12ModelReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\"\x17\n\x15ServerMetadataRequest\"K\n\x16ServerMetadataResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x12\n\nextensions\x18\x03 \x03(\t\"5\n\x14ModelMetadataRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"\x93\x02\n\x15ModelMetadataResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08versions\x18\x02 \x03(\t\x12\x10\n\x08platform\x18\x03 \x01(\t\x12\x42\n\x06inputs\x18\x04 \x03(\x0b\x32\x32.taichu_infer.ModelMetadataResponse.TensorMetadata\x12\x43\n\x07outputs\x18\x05 \x03(\x0b\x32\x32.taichu_infer.ModelMetadataResponse.TensorMetadata\x1a?\n\x0eTensorMetadata\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05shape\x18\x03 \x03(\x03\"\xbe\x03\n\x11ModelInferRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x43\n\nparameters\x18\x04 \x03(\x0b\x32/.taichu_infer.ModelInferRequest.ParametersEntry\x1a\xdb\x01\n\x1aInferRequestedOutputTensor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12^\n\nparameters\x18\x02 \x03(\x0b\x32J.taichu_infer.ModelInferRequest.InferRequestedOutputTensor.ParametersEntry\x1aO\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.taichu_infer.InferParameter:\x02\x38\x01\x1aO\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.taichu_infer.InferParameter:\x02\x38\x01\"\xe2\x01\n\x12ModelInferResponse\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x44\n\nparameters\x18\x04 \x03(\x0b\x32\x30.taichu_infer.ModelInferResponse.ParametersEntry\x1aO\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.taichu_infer.InferParameter:\x02\x38\x01\"\x80\x01\n\x0eInferParameter\x12\x14\n\nbool_param\x18\x01 \x01(\x08H\x00\x12\x15\n\x0bint64_param\x18\x02 \x01(\x03H\x00\x12\x15\n\x0b\x66loat_param\x18\x03 \x01(\x02H\x00\x12\x16\n\x0cstring_param\x18\x04 \x01(\tH\x00\x42\x12\n\x10parameter_choice2\xfd\x04\n\x14GRPCInferenceService\x12Q\n\nServerLive\x12\x1f.taichu_infer.ServerLiveRequest\x1a .taichu_infer.ServerLiveResponse\"\x00\x12T\n\x0bServerReady\x12 .taichu_infer.ServerReadyRequest\x1a!.taichu_infer.ServerReadyResponse\"\x00\x12Q\n\nModelReady\x12\x1f.taichu_infer.ModelReadyRequest\x1a .taichu_infer.ModelReadyResponse\"\x00\x12]\n\x0eServerMetadata\x12#.taichu_infer.ServerMetadataRequest\x1a$.taichu_infer.ServerMetadataResponse\"\x00\x12Z\n\rModelMetadata\x12\".taichu_infer.ModelMetadataRequest\x1a#.taichu_infer.ModelMetadataResponse\"\x00\x12Q\n\nModelInfer\x12\x1f.taichu_infer.ModelInferRequest\x1a .taichu_infer.ModelInferResponse\"\x00\x12[\n\x10ModelStreamInfer\x12\x1f.taichu_infer.ModelInferRequest\x1a .taichu_infer.ModelInferResponse\"\x00(\x01\x30\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15grpc_predict_v2.proto\x12\x0ctaichu_infer\"\x13\n\x11ServerLiveRequest\"\"\n\x12ServerLiveResponse\x12\x0c\n\x04live\x18\x01 \x01(\x08\"\x14\n\x12ServerReadyRequest\"$\n\x13ServerReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\"2\n\x11ModelReadyRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"#\n\x12ModelReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\"\x17\n\x15ServerMetadataRequest\"K\n\x16ServerMetadataResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x12\n\nextensions\x18\x03 \x03(\t\"5\n\x14ModelMetadataRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"\x93\x02\n\x15ModelMetadataResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08versions\x18\x02 \x03(\t\x12\x10\n\x08platform\x18\x03 \x01(\t\x12\x42\n\x06inputs\x18\x04 \x03(\x0b\x32\x32.taichu_infer.ModelMetadataResponse.TensorMetadata\x12\x43\n\x07outputs\x18\x05 \x03(\x0b\x32\x32.taichu_infer.ModelMetadataResponse.TensorMetadata\x1a?\n\x0eTensorMetadata\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05shape\x18\x03 \x03(\x03\"\xbe\x03\n\x11ModelInferRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x43\n\nparameters\x18\x04 \x03(\x0b\x32/.taichu_infer.ModelInferRequest.ParametersEntry\x1a\xdb\x01\n\x1aInferRequestedOutputTensor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12^\n\nparameters\x18\x02 \x03(\x0b\x32J.taichu_infer.ModelInferRequest.InferRequestedOutputTensor.ParametersEntry\x1aO\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.taichu_infer.InferParameter:\x02\x38\x01\x1aO\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.taichu_infer.InferParameter:\x02\x38\x01\"\xe2\x01\n\x12ModelInferResponse\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x44\n\nparameters\x18\x04 \x03(\x0b\x32\x30.taichu_infer.ModelInferResponse.ParametersEntry\x1aO\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.taichu_infer.InferParameter:\x02\x38\x01\"i\n\x0eInferParameter\x12\x14\n\nbool_param\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x66loat_param\x18\x02 \x01(\x02H\x00\x12\x16\n\x0cstring_param\x18\x03 \x01(\tH\x00\x42\x12\n\x10parameter_choice2\xfd\x04\n\x14GRPCInferenceService\x12Q\n\nServerLive\x12\x1f.taichu_infer.ServerLiveRequest\x1a .taichu_infer.ServerLiveResponse\"\x00\x12T\n\x0bServerReady\x12 .taichu_infer.ServerReadyRequest\x1a!.taichu_infer.ServerReadyResponse\"\x00\x12Q\n\nModelReady\x12\x1f.taichu_infer.ModelReadyRequest\x1a .taichu_infer.ModelReadyResponse\"\x00\x12]\n\x0eServerMetadata\x12#.taichu_infer.ServerMetadataRequest\x1a$.taichu_infer.ServerMetadataResponse\"\x00\x12Z\n\rModelMetadata\x12\".taichu_infer.ModelMetadataRequest\x1a#.taichu_infer.ModelMetadataResponse\"\x00\x12Q\n\nModelInfer\x12\x1f.taichu_infer.ModelInferRequest\x1a .taichu_infer.ModelInferResponse\"\x00\x12[\n\x10ModelStreamInfer\x12\x1f.taichu_infer.ModelInferRequest\x1a .taichu_infer.ModelInferResponse\"\x00(\x01\x30\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpc_predict_v2_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _MODELINFERREQUEST_INFERREQUESTEDOUTPUTTENSOR_PARAMETERSENTRY._options = None
@@ -56,12 +56,12 @@
   _MODELINFERREQUEST_INFERREQUESTEDOUTPUTTENSOR_PARAMETERSENTRY._serialized_end=1046
   _MODELINFERREQUEST_PARAMETERSENTRY._serialized_start=967
   _MODELINFERREQUEST_PARAMETERSENTRY._serialized_end=1046
   _MODELINFERRESPONSE._serialized_start=1130
   _MODELINFERRESPONSE._serialized_end=1356
   _MODELINFERRESPONSE_PARAMETERSENTRY._serialized_start=967
   _MODELINFERRESPONSE_PARAMETERSENTRY._serialized_end=1046
-  _INFERPARAMETER._serialized_start=1359
-  _INFERPARAMETER._serialized_end=1487
-  _GRPCINFERENCESERVICE._serialized_start=1490
-  _GRPCINFERENCESERVICE._serialized_end=2127
+  _INFERPARAMETER._serialized_start=1358
+  _INFERPARAMETER._serialized_end=1463
+  _GRPCINFERENCESERVICE._serialized_start=1466
+  _GRPCINFERENCESERVICE._serialized_end=2103
 # @@protoc_insertion_point(module_scope)
```

### Comparing `taichu-serve-1.0.11/model_service/grpc_predict_v2_pb2_grpc.py` & `taichu-serve-2.0.2/taichu_serve/grpc_predict_v2_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-import grpc_predict_v2_pb2 as grpc__predict__v2__pb2
+import taichu_serve.grpc_predict_v2_pb2 as grpc__predict__v2__pb2
 
 
 class GRPCInferenceServiceStub(object):
     """Inference Server GRPC endpoints.
     """
 
     def __init__(self, channel):
```

### Comparing `taichu-serve-1.0.11/model_service/grpc_server.py` & `taichu-serve-2.0.2/taichu_serve/grpc_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import logging
 import traceback
+import uuid
 
 from grpc import RpcError
 
-import grpc_predict_v2_pb2_grpc
-import grpc_predict_v2_pb2
-from app import get_model_service
+import taichu_serve.grpc_predict_v2_pb2_grpc as grpc_predict_v2_pb2_grpc
+import taichu_serve.grpc_predict_v2_pb2 as grpc_predict_v2_pb2
+from taichu_serve.app import model_inference
 
-from error_code import ModelNotFoundError, ModelPredictError
-from common import grpc_interceptor
+from taichu_serve.error_code import ModelNotFoundError, ModelPredictError
+from taichu_serve.common import grpc_interceptor
 
 logger = logging.getLogger(__name__)
 
 
 def parameters_to_dict(parameters):
     dic = {}
 
     for key, value in parameters.items():
-        if value.HasField('int64_param'):
-            dic[key] = value.int64_param
-        elif value.HasField('bool_param'):
+        if value.HasField('bool_param'):
             dic[key] = value.bool_param
         elif value.HasField('float_param'):
             dic[key] = value.float_param
         elif value.HasField('string_param'):
             dic[key] = value.string_param
         else:
             print('error type: ', type(value))
@@ -40,68 +39,67 @@
         resp = grpc_predict_v2_pb2.ModelInferResponse()
 
         if dic is None:
             return resp
 
         for key, value in dic.items():
             if type(value) == int:
-                resp.parameters[key].int64_param = value
+                resp.parameters[key].float_param = float(value)
             elif type(value) == bool:
                 resp.parameters[key].bool_param = value
             elif type(value) == float:
                 resp.parameters[key].float_param = value
             elif type(value) == str:
                 resp.parameters[key].string_param = value
             else:
                 print('error type: ', type(value))
 
         return resp
 
     @grpc_interceptor
     def ModelInfer(self, request, context):
-        ctx = {}
+        request_id = str(uuid.uuid4())
         rec_dict = parameters_to_dict(request.parameters)
-        instance = get_model_service(request.model_name, request.model_version)
         try:
-            ret = instance.inference(rec_dict, context=ctx)
+            ret = model_inference(request.model_name, request.model_version, rec_dict, request_id)
         except Exception as e:
             logger.error('Algorithm crashed!')
             logger.error(traceback.format_exc())
             raise ModelPredictError(message=str(e))
         resp = self.make_response(ret)
         resp.model_name = request.model_name
         resp.model_version = request.model_version
+        resp.id = request.id
 
         return resp
 
     @grpc_interceptor
     def ModelStreamInfer(self, request, context):
         # 检测是否有客户端断开连接
-        ctx = {}
+        request_id = str(uuid.uuid4())
+
         while context.is_active():
             for req in request:
-                # logger.info('recv: %s', req)
-                ctx['model_name'] = req.model_name
-                ctx['model_version'] = req.model_version
-
-                instance = get_model_service(req.model_name, req.model_version)
+                logger.info('recv a request')
+                if req.id and len(req.id) > 0:
+                    request_id = req.id
 
                 rec_dict = parameters_to_dict(req.parameters)
-
                 try:
-                    res = instance.inference(rec_dict, context=ctx)
+                    res = model_inference(req.model_name, req.model_version, rec_dict, request_id)
                 except Exception as e:
                     logger.error('Algorithm crashed!, %s', str(e))
                     logger.error(traceback.format_exc())
                     raise ModelPredictError(message=str(e))
 
-                # logger.info('ret: %s', res)
+
                 resp = self.make_response(res)
                 resp.model_name = req.model_name
                 resp.model_version = req.model_version
+                resp.id = request_id
 
                 yield resp
 
     def ServerLive(self, request, context):
         resp = grpc_predict_v2_pb2.ServerLiveResponse(
             live=True,
         )
```

### Comparing `taichu-serve-1.0.11/model_service/log.py` & `taichu-serve-2.0.2/taichu_serve/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import sys
 from typing import Optional
 
 from flask import request, g
-from common import Local
+from taichu_serve.common import Local
 
 class JsonFormatter(logging.Formatter):
 
     def __init__(
             self,
             fmt: Optional[str] = "%(asctime)s",
             datefmt: Optional[str] = None,
```

### Comparing `taichu-serve-1.0.11/model_service/model_service.py` & `taichu-serve-2.0.2/taichu_serve/model_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 import traceback
 from abc import ABCMeta, abstractmethod
 import time
 
 logger = logging.getLogger(__name__)
 
 
-class ModelService(object):
+class BaseModelService(object):
     '''ModelService wraps up all preprocessing, inference and postprocessing
     functions used by model service. It is defined in a flexible manner to
     be easily extended to support different frameworks.
     '''
     __metaclass__ = ABCMeta
 
     def __init__(self, model_path):
         self.ctx = None
 
     @abstractmethod
-    def inference(self, data, context={}):
+    def inference(self, data, request_id):
         '''
         Wrapper function to run preprocess, inference and postprocess functions.
 
         Parameters
         ----------
         data : map of object
             Raw input from request.
@@ -58,131 +58,131 @@
         -------
         Dict
             Model service signiture.
         '''
         pass
 
 
-class SingleNodeService(ModelService):
-    '''SingleNodeModel defines abstraction for model service which loads a
-    single model.
-    '''
-
-    def __init__(self, model_path):
-        super(SingleNodeService, self).__init__(model_path)
-        self._ready = False
-
-    def warmup(self):
-        start_time = time.time()
-        self._warmup()
-        self._ready = True
-        logger.info('warmup time: ' + str((time.time() - start_time) * 1000) + 'ms')
-
-    def inference(self, data, context={}):
-        '''
-        Wrapper function to run preprocess, inference and postprocess functions.
-
-        Parameters
-        ----------
-        data : map of object
-            Raw input from request.
-
-        Returns
-        -------
-        list of outputs to be sent back to client.
-            data to be sent back
-        '''
-        pre_start_time = time.time()
-        data = self._preprocess(data, context=context)
-        infer_start_time = time.time()
-
-        # Update preprocess latency metric
-        pre_time_in_ms = (infer_start_time - pre_start_time) * 1000
-        logger.info('preprocess time: ' + str(pre_time_in_ms) + 'ms')
-
-        data = self._inference(data, context=context)
-        infer_end_time = time.time()
-        infer_in_ms = (infer_end_time - infer_start_time) * 1000
-
-        logger.info('infer time: ' + str(infer_in_ms) + 'ms')
-        data = self._postprocess(data, context=context)
-
-        # Update inference latency metric
-        post_time_in_ms = (time.time() - infer_end_time) * 1000
-        logger.info('postprocess time: ' + str(post_time_in_ms) + 'ms')
-
-        logger.info('latency: ' + str(pre_time_in_ms + infer_in_ms + post_time_in_ms) + 'ms')
-        return data
-
-    @abstractmethod
-    def _inference(self, data, context={}):
-        '''
-        Internal inference methods. Run forward computation and
-        return output.
-
-        Parameters
-        ----------
-        data : map of NDArray
-            Preprocessed inputs in NDArray format.
-
-        Returns
-        -------
-        list of NDArray
-            Inference output.
-        '''
-        return data
-
-    @abstractmethod
-    def _preprocess(self, data, context={}):
-        '''
-        Internal preprocess methods. Do transformation on raw
-        inputs and convert them to NDArray.
-
-        Parameters
-        ----------
-        data : map of object
-            Raw inputs from request.
-
-        Returns
-        -------
-        list of NDArray
-            Processed inputs in NDArray format.
-        '''
-        return data
-
-    @abstractmethod
-    def _postprocess(self, data, context={}):
-        '''
-        Internal postprocess methods. Do transformation on inference output
-        and convert them to MIME type objects.
-
-        Parameters
-        ----------
-        data : map of NDArray
-            Inference output.
-
-        Returns
-        -------
-        list of object
-            list of outputs to be sent back.
-        '''
-        return data
-
-    @abstractmethod
-    def _warmup(self):
-        pass
-
-    @property
-    def model_version(self):
-        return '1'
-
-    @property
-    def ready(self):
-        return self._ready
-
+# class SingleNodeService(BaseModelService):
+#     '''SingleNodeModel defines abstraction for model service which loads a
+#     single model.
+#     '''
+#
+#     def __init__(self, model_path):
+#         super(SingleNodeService, self).__init__(model_path)
+#         self._ready = False
+#
+#     def warmup(self):
+#         start_time = time.time()
+#         self._warmup()
+#         self._ready = True
+#         logger.info('warmup time: ' + str((time.time() - start_time) * 1000) + 'ms')
+#
+#     def inference(self, data, context={}):
+#         '''
+#         Wrapper function to run preprocess, inference and postprocess functions.
+#
+#         Parameters
+#         ----------
+#         data : map of object
+#             Raw input from request.
+#
+#         Returns
+#         -------
+#         list of outputs to be sent back to client.
+#             data to be sent back
+#         '''
+#         pre_start_time = time.time()
+#         data = self._preprocess(data, context=context)
+#         infer_start_time = time.time()
+#
+#         # Update preprocess latency metric
+#         pre_time_in_ms = (infer_start_time - pre_start_time) * 1000
+#         logger.info('preprocess time: ' + str(pre_time_in_ms) + 'ms')
+#
+#         data = self._inference(data, context=context)
+#         infer_end_time = time.time()
+#         infer_in_ms = (infer_end_time - infer_start_time) * 1000
+#
+#         logger.info('infer time: ' + str(infer_in_ms) + 'ms')
+#         data = self._postprocess(data, context=context)
+#
+#         # Update inference latency metric
+#         post_time_in_ms = (time.time() - infer_end_time) * 1000
+#         logger.info('postprocess time: ' + str(post_time_in_ms) + 'ms')
+#
+#         logger.info('latency: ' + str(pre_time_in_ms + infer_in_ms + post_time_in_ms) + 'ms')
+#         return data
+#
+#     @abstractmethod
+#     def _inference(self, data, context={}):
+#         '''
+#         Internal inference methods. Run forward computation and
+#         return output.
+#
+#         Parameters
+#         ----------
+#         data : map of NDArray
+#             Preprocessed inputs in NDArray format.
+#
+#         Returns
+#         -------
+#         list of NDArray
+#             Inference output.
+#         '''
+#         return data
+#
+#     @abstractmethod
+#     def _preprocess(self, data, context={}):
+#         '''
+#         Internal preprocess methods. Do transformation on raw
+#         inputs and convert them to NDArray.
+#
+#         Parameters
+#         ----------
+#         data : map of object
+#             Raw inputs from request.
+#
+#         Returns
+#         -------
+#         list of NDArray
+#             Processed inputs in NDArray format.
+#         '''
+#         return data
+#
+#     @abstractmethod
+#     def _postprocess(self, data, context={}):
+#         '''
+#         Internal postprocess methods. Do transformation on inference output
+#         and convert them to MIME type objects.
+#
+#         Parameters
+#         ----------
+#         data : map of NDArray
+#             Inference output.
+#
+#         Returns
+#         -------
+#         list of object
+#             list of outputs to be sent back.
+#         '''
+#         return data
+#
+#     @abstractmethod
+#     def _warmup(self):
+#         pass
+#
+#     @property
+#     def model_version(self):
+#         return '1'
+#
+#     @property
+#     def ready(self):
+#         return self._ready
+#
 
 def load_service(path, name=None):
     sys.path.append(os.path.dirname(path))
 
     try:
         if not name:
             name = os.path.splitext(os.path.basename(path))[0]
```

### Comparing `taichu-serve-1.0.11/setup.py` & `taichu-serve-2.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from datetime import date
 import sys
 from setuptools import setup, find_packages
 # pylint: disable = relative-import
-import model_service
+import taichu_serve
 
 pkgs = find_packages()
 
 if __name__ == '__main__':
     name = 'taichu-serve'
 
     requirements = ['grpcio', 'grpcio-tools', 'protobuf', 'Flask', 'gunicorn', 'Jinja2', 'Pillow']
 
     setup(
         name=name,
-        version='1.0.11',
+        version='2.0.2',
         description='taichu serve is a tool for serving deep learning inference',
         # long_description='',
         author='taichu platform team',
         # author_email='noreply@noreply.com',
         python_requires=">=3.6.0",
         url='',
         keywords='Serving Deep Learning Inference AI',
         packages=pkgs,
         install_requires=requirements,
         entry_points={
-            'console_scripts': ['taichu-serve = model_service.command:infer_server_start']
+            'console_scripts': ['taichu_serve = taichu_serve.command:infer_server_start']
         },
         include_package_data=True,
         # license='Apache License Version 2.0'
     )
```

