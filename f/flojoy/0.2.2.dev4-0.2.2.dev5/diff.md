# Comparing `tmp/flojoy-0.2.2.dev4.tar.gz` & `tmp/flojoy-0.2.2.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flojoy-0.2.2.dev4.tar", last modified: Thu Apr 13 00:20:29 2023, max compression
+gzip compressed data, was "flojoy-0.2.2.dev5.tar", last modified: Thu Apr 13 22:56:10 2023, max compression
```

## Comparing `flojoy-0.2.2.dev4.tar` & `flojoy-0.2.2.dev5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-13 00:20:29.369062 flojoy-0.2.2.dev4/
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1062 2022-10-05 16:22:32.000000 flojoy-0.2.2.dev4/LICENSE.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-13 00:20:29.369062 flojoy-0.2.2.dev4/PKG-INFO
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       31 2022-10-05 16:21:51.000000 flojoy-0.2.2.dev4/README.md
-drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-13 00:20:29.369062 flojoy-0.2.2.dev4/flojoy/
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      188 2023-04-03 20:53:50.000000 flojoy-0.2.2.dev4/flojoy/__init__.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      209 2023-04-04 16:27:03.000000 flojoy-0.2.2.dev4/flojoy/flojoy_instruction.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)    19528 2023-04-13 00:12:11.000000 flojoy-0.2.2.dev4/flojoy/flojoy_python.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     3024 2023-04-13 00:13:32.000000 flojoy-0.2.2.dev4/flojoy/job_result_builder.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     2128 2023-04-13 00:09:10.000000 flojoy-0.2.2.dev4/flojoy/job_result_utils.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     2368 2023-04-13 00:14:51.000000 flojoy-0.2.2.dev4/flojoy/plotly_utils.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     6070 2023-02-20 19:12:45.000000 flojoy-0.2.2.dev4/flojoy/utils.py
-drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-13 00:20:29.369062 flojoy-0.2.2.dev4/flojoy.egg-info/
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-13 00:20:29.000000 flojoy-0.2.2.dev4/flojoy.egg-info/PKG-INFO
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      356 2023-04-13 00:20:29.000000 flojoy-0.2.2.dev4/flojoy.egg-info/SOURCES.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        1 2023-04-13 00:20:29.000000 flojoy-0.2.2.dev4/flojoy.egg-info/dependency_links.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       76 2023-04-13 00:20:29.000000 flojoy-0.2.2.dev4/flojoy.egg-info/requires.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        7 2023-04-13 00:20:29.000000 flojoy-0.2.2.dev4/flojoy.egg-info/top_level.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       79 2023-04-13 00:20:29.369062 flojoy-0.2.2.dev4/setup.cfg
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      956 2023-04-13 00:08:08.000000 flojoy-0.2.2.dev4/setup.py
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-13 22:56:10.019645 flojoy-0.2.2.dev5/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1062 2022-10-05 16:22:32.000000 flojoy-0.2.2.dev5/LICENSE.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-13 22:56:10.019645 flojoy-0.2.2.dev5/PKG-INFO
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       31 2022-10-05 16:21:51.000000 flojoy-0.2.2.dev5/README.md
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-13 22:56:10.015645 flojoy-0.2.2.dev5/flojoy/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      188 2023-04-03 20:53:50.000000 flojoy-0.2.2.dev5/flojoy/__init__.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      209 2023-04-04 16:27:03.000000 flojoy-0.2.2.dev5/flojoy/flojoy_instruction.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)    19695 2023-04-13 22:54:52.000000 flojoy-0.2.2.dev5/flojoy/flojoy_python.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     2132 2023-04-13 22:49:50.000000 flojoy-0.2.2.dev5/flojoy/job_result_builder.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1725 2023-04-13 22:53:14.000000 flojoy-0.2.2.dev5/flojoy/job_result_utils.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1186 2023-04-13 22:51:34.000000 flojoy-0.2.2.dev5/flojoy/plotly_utils.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     6070 2023-02-20 19:12:45.000000 flojoy-0.2.2.dev5/flojoy/utils.py
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-13 22:56:10.019645 flojoy-0.2.2.dev5/flojoy.egg-info/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-13 22:56:09.000000 flojoy-0.2.2.dev5/flojoy.egg-info/PKG-INFO
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      356 2023-04-13 22:56:09.000000 flojoy-0.2.2.dev5/flojoy.egg-info/SOURCES.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        1 2023-04-13 22:56:09.000000 flojoy-0.2.2.dev5/flojoy.egg-info/dependency_links.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       76 2023-04-13 22:56:09.000000 flojoy-0.2.2.dev5/flojoy.egg-info/requires.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        7 2023-04-13 22:56:09.000000 flojoy-0.2.2.dev5/flojoy.egg-info/top_level.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       79 2023-04-13 22:56:10.019645 flojoy-0.2.2.dev5/setup.cfg
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      956 2023-04-13 22:55:44.000000 flojoy-0.2.2.dev5/setup.py
```

### Comparing `flojoy-0.2.2.dev4/LICENSE.txt` & `flojoy-0.2.2.dev5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flojoy-0.2.2.dev4/PKG-INFO` & `flojoy-0.2.2.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flojoy
-Version: 0.2.2.dev4
+Version: 0.2.2.dev5
 Summary: Python client library for Flojoy.
 Home-page: https://github.com/flojoy-io/flojoy-python
 Author: flojoy
 Author-email: jack.parmer@proton.me
 License: MIT
 Download-URL: https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip
 Keywords: data-acquisition,lab-automation,low-code,python,scheduler,topic
```

### Comparing `flojoy-0.2.2.dev4/flojoy/flojoy_python.py` & `flojoy-0.2.2.dev5/flojoy/flojoy_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from redis import Redis
 from rq.job import Job
 import os
 from functools import wraps
 from .utils import PlotlyJSONEncoder, dump_str
 import requests
 from dotenv import dotenv_values
-from .job_result_utils import get_data, get_data_container_output
+from .job_result_utils import get_result, get_data_container_obj
 
 
 port = dotenv_values().get('REACT_APP_BACKEND_PORT', '8000')
 
 REDIS_HOST = os.environ.get('REDIS_HOST', 'localhost')
 REDIS_PORT = os.environ.get('REDIS_PORT', 6379)
 BACKEND_HOST = os.environ.get('BACKEND_HOST', 'localhost')
@@ -40,27 +40,27 @@
     v.y = np.sin(v.x)
     v.type = 'ordered_pair'
 
     '''
     allowed_types = ['grayscale', 'matrix', 'dataframe',
                      'image', 'ordered_pair', 'ordered_triple', 'scalar', 'plotly']
     allowed_keys = ['x', 'y', 'z', 't', 'm',
-                    'c', 'r', 'g', 'b', 'a','f']
+                    'c', 'r', 'g', 'b', 'a','fig']
     combinations = {
         'x': ['y', 't', 'z'],
         'y': ['x', 't', 'z'],
         'z': ['x', 'y', 't'],
         'c': ['t'],
         'm': ['t'],
-        't':  [value for value in allowed_keys if value not in ['t']],
+        't':  [*(value for value in allowed_keys if value not in ['t'])],
         'r': ['g', 'b', 't', 'a'],
         'g': ['r', 'b', 't', 'a'],
         'b': ['r', 'g', 't', 'a'],
         'a': ['r', 'g', 'b', 't'],
-        'f': []
+        'fig': [*(k for k in allowed_keys if k not in ['fig'])]
     }
 
     def _ndarrayify(self, value):
         s = str(type(value))
         v_type = s.split("'")[1]
 
         match v_type:
@@ -116,19 +116,21 @@
             case 'scalar':
                 if 'c' not in kwargs:
                     raise KeyError(
                         f'c key must be provided for type "{data_type}"')
                 else:
                     self['c'] = kwargs['c']
             case 'plotly':
-                if 'f' not in kwargs:
+                if 'fig' not in kwargs:
                     raise KeyError(
                         f'f key must be provided for type "{data_type}"')
                 else:
-                    self['f'] = kwargs['f']
+                    for k, value in kwargs.items():
+                        self[k] = value
+                    
             case _:
                 if data_type.startswith('parametric_'):
                     if 't' not in kwargs:
                         raise KeyError(
                             f't key must be provided for "{data_type}"')
                     self['t'] = kwargs['t']
                     t = kwargs['t']
@@ -159,15 +161,15 @@
             case 'ordered_triple':
                 if key not in ['x', 'y', 'z']:
                     raise KeyError(self.build_error_text(key, data_type))
             case 'scalar':
                 if key not in ['c']:
                     raise KeyError(self.build_error_text(key, data_type))
             case 'plotly':
-                if key not in ['f']:
+                if key not in ['fig', *(k for k in self.combinations['fig'])]:
                     raise KeyError(self.build_error_text(key, data_type))
 
     def set_data(self, data_type: str, key: str, value, isType: bool):
         if data_type not in self.allowed_types and data_type.startswith('parametric_'):
             if 't' not in self:
                 if key != 't':
                     raise KeyError(
@@ -195,15 +197,15 @@
 
                 super().__setitem__(key, array)
                 return
         elif data_type in self.allowed_types:
             self.validate_key(data_type, key)
             if isType:
                 return
-            formatted_value = self._ndarrayify(value) if data_type != 'plotly' else value
+            formatted_value = self._ndarrayify(value) if key != 'fig' else value
             super().__setitem__(key, formatted_value)
         else:
             raise ValueError(
                 f'Invalid data type "{data_type}"')
 
     def __init__(self, **kwargs):
         if 'type' in kwargs:
@@ -240,15 +242,15 @@
 
                     if key in self.combinations.keys():
                         self.check_combination(
                             key, has_keys, self.combinations[key])
                         super().__setitem__(key, value)
                         return
                 else:
-                    formatted_value = self._ndarrayify(value) if key != 'f' else value
+                    formatted_value = self._ndarrayify(value) if key != 'fig' else value
                     super().__setitem__(key, formatted_value)
                     return
         else:
             has_any_key = False
             has_keys = []
             for i in self.allowed_keys:
                 if hasattr(self, i):
@@ -316,15 +318,15 @@
     inputs = []
     redis_connection = Redis(host=REDIS_HOST, port=REDIS_PORT)
 
     try:
         for prev_job_id in previous_job_ids:
             print('fetching input from prev job id:', prev_job_id)
             job = Job.fetch(prev_job_id, connection=redis_connection)
-            result = get_data_container_output(job.result)
+            result = get_data_container_obj(job.result)
             print('fetch input from prev job id:', prev_job_id,
                   ' result:', dump_str(result, limit=100))
             inputs.append(result)
     except Exception:
         print(traceback.format_exc())
 
     return inputs
@@ -423,35 +425,34 @@
             func_params['node_id'] = node_id
             func_params['job_id'] = job_id
 
             print('executing node_id:', node_id,
                   'previous_job_ids:', previous_job_ids)
             print(node_id, ' params: ', json.dumps(func_params, indent=2))
             node_inputs = fetch_inputs(previous_job_ids, mock)
-            result = func(node_inputs, func_params)
-            data = get_data(result)
+            dt_obj = func(node_inputs, func_params) # DataContainer object from node
+            result = get_result(dt_obj)
             send_to_socket(json.dumps({
                 'NODE_RESULTS': {
                     'cmd': FN,
                     'id': node_id,
-                    'result': data['result'],
+                    'result': result,
                 },
                 'jobsetId': jobset_id
             }, cls=PlotlyJSONEncoder))
 
             if func.__name__ == 'END':
                 send_to_socket(json.dumps({
                     'SYSTEM_STATUS': '🤙 python script run successful',
                     'RUNNING_NODE': '',
                     'jobsetId': jobset_id
                 }))
 
-            print('final result:', dump_str(data['output'], limit=100))
-
-            return data['output']
+            print('final result:', dump_str(result, limit=100))
+            return result
         except Exception as e:
             send_to_socket(json.dumps({
                 'SYSTEM_STATUS': f'Failed to run: {func.__name__}',
                 'FAILED_NODES': node_id,
                 'FAILURE_REASON': e.args[0],
                 'jobsetId': jobset_id
             }))
```

### Comparing `flojoy-0.2.2.dev4/flojoy/job_result_builder.py` & `flojoy-0.2.2.dev5/flojoy/job_result_builder.py`

 * *Files 18% similar despite different names*

```diff
@@ -62,34 +62,12 @@
                 # instructions to job scheduler (watch.py)
                 **self.instructions,
                 # instruction to fetch_input method in flojoy.py
                 FLOJOY_INSTRUCTION.RESULT_FIELD: "data",
                 'data': result,
             }
         return result
-    class To_plot_args(TypedDict):
-        plot_type: str
-        fig: Figure
-        data_container_plotly: DataContainer
-        
-    def to_plot(self, args: To_plot_args):
-        if not self.instructions:
-            self.instructions = {}
-        if args.get('fig', None) is not None:
-            fig = args['fig'] # get_plot_fig_by_type(plot_type=plot_type, **kwargs)
-            output = fig.to_dict()
-        elif args.get('data_container_plotly',None) is not None:
-            output = data_container_to_plotly(args['data_container_plotly'], None)
-        else:
-            output = data_container_to_plotly(self.data, plot_type=args['plot_type'])
 
-        return {
-            **self.instructions,
-            FLOJOY_INSTRUCTION.DATACONTAINER_FIELD: 'result',
-            'result': self.data,
-            FLOJOY_INSTRUCTION.RESULT_FIELD: 'data',
-            'data': output
-        }
     def get_default_data(self):
         x = np.arange(0,1000,1)
         y = np.ones_like(x)
         return DataContainer(x=x, y=y)
```

### Comparing `flojoy-0.2.2.dev4/flojoy/job_result_utils.py` & `flojoy-0.2.2.dev5/flojoy/job_result_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,49 +18,40 @@
     return result.get(FLOJOY_INSTRUCTION.FLOW_TO_DIRECTIONS, ['main'])
 
 
 def get_next_nodes(result):
     if result is None: return []
     return result.get(FLOJOY_INSTRUCTION.FLOW_TO_NODES, [])
 
-def get_data_container_output(result):
+def get_data_container_obj(result):
     if not result:
         return {}
-    if result.get(FLOJOY_INSTRUCTION.DATACONTAINER_FIELD): # to_plot is used
-        return result[result[FLOJOY_INSTRUCTION.DATACONTAINER_FIELD]]
     if result.get(FLOJOY_INSTRUCTION.RESULT_FIELD):
         return result[result[FLOJOY_INSTRUCTION.RESULT_FIELD]]
-    return result
+    return result['data']
 
 def get_job_result(job_id: str):
         job = Job.fetch(job_id, connection=Redis(
             host=REDIS_HOST, port=REDIS_PORT))
-        result = get_data_container_output(job.result)
+        result = get_data_container_obj(job.result)
         return result
-    
 
 
-
-def get_data(result):
+def get_result(result):
     if not result:
         return {
-            'output': result,
-            'result': result
-        }
-    if result.get(FLOJOY_INSTRUCTION.DATACONTAINER_FIELD): # to_plot is used
-        data = result[result[FLOJOY_INSTRUCTION.RESULT_FIELD]] # already processed for plotly
-        return {
-            'output': result,
-            'result': data
+            'default_fig': result,
+            'data': result
         }
     if result.get(FLOJOY_INSTRUCTION.RESULT_FIELD):
-        data_container = result[result[FLOJOY_INSTRUCTION.RESULT_FIELD]]
-        data = data_container_to_plotly(data=data_container, plot_type=None)
+        data = result[result[FLOJOY_INSTRUCTION.RESULT_FIELD]]
+        plotly_fig = data_container_to_plotly(data=data)
         return {
-            'output':result,
-            'result': data
+            **result,
+            'default_fig':plotly_fig,
+            'data': data
         }
-    data = data_container_to_plotly(data=result, plot_type=None)
+    plotly_fig = data_container_to_plotly(data=result)
     return {
-        'output': result,
-        'result': data
+        'default_fig': plotly_fig,
+        'data': result
     }
```

### Comparing `flojoy-0.2.2.dev4/flojoy/utils.py` & `flojoy-0.2.2.dev5/flojoy/utils.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.2.2.dev4/flojoy.egg-info/PKG-INFO` & `flojoy-0.2.2.dev5/flojoy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flojoy
-Version: 0.2.2.dev4
+Version: 0.2.2.dev5
 Summary: Python client library for Flojoy.
 Home-page: https://github.com/flojoy-io/flojoy-python
 Author: flojoy
 Author-email: jack.parmer@proton.me
 License: MIT
 Download-URL: https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip
 Keywords: data-acquisition,lab-automation,low-code,python,scheduler,topic
```

### Comparing `flojoy-0.2.2.dev4/setup.py` & `flojoy-0.2.2.dev5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 setup(
     name='flojoy',
     packages=['flojoy'],
-    version='0.2.2.dev4',
+    version='0.2.2.dev5',
     license='MIT',
     description='Python client library for Flojoy.',
     author='flojoy',
     author_email='jack.parmer@proton.me',
     url='https://github.com/flojoy-io/flojoy-python',
     download_url='https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip',
     keywords=['data-acquisition', 'lab-automation', 'low-code', 'python', 'scheduler', 'topic'],
```

