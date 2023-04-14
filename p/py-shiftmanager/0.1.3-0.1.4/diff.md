# Comparing `tmp/py_shiftmanager-0.1.3.tar.gz` & `tmp/py_shiftmanager-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_shiftmanager-0.1.3.tar", last modified: Thu Apr 13 12:13:58 2023, max compression
+gzip compressed data, was "py_shiftmanager-0.1.4.tar", last modified: Fri Apr 14 14:16:37 2023, max compression
```

## Comparing `py_shiftmanager-0.1.3.tar` & `py_shiftmanager-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-13 12:13:58.550831 py_shiftmanager-0.1.3/
--rw-r--r--   0 amitnakash   (501) staff       (20)       17 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.3/MANIFEST.in
--rw-r--r--   0 amitnakash   (501) staff       (20)     8033 2023-04-13 12:13:58.550680 py_shiftmanager-0.1.3/PKG-INFO
--rw-r--r--   0 amitnakash   (501) staff       (20)     7714 2023-04-13 12:08:22.000000 py_shiftmanager-0.1.3/Readme.md
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-13 12:13:58.549677 py_shiftmanager-0.1.3/py_shiftmanager/
--rw-r--r--   0 amitnakash   (501) staff       (20)      289 2023-04-13 06:10:21.000000 py_shiftmanager-0.1.3/py_shiftmanager/__init__.py
--rw-r--r--   0 amitnakash   (501) staff       (20)      428 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.3/py_shiftmanager/logger.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     4794 2023-04-13 12:06:40.000000 py_shiftmanager-0.1.3/py_shiftmanager/shiftmanager_compute.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     5025 2023-04-13 12:06:42.000000 py_shiftmanager-0.1.3/py_shiftmanager/shiftmanager_io.py
--rw-r--r--   0 amitnakash   (501) staff       (20)      782 2023-04-13 05:47:37.000000 py_shiftmanager-0.1.3/py_shiftmanager/timeout.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     3272 2023-04-13 11:21:29.000000 py_shiftmanager-0.1.3/py_shiftmanager/worker.py
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-13 12:13:58.550434 py_shiftmanager-0.1.3/py_shiftmanager.egg-info/
--rw-r--r--   0 amitnakash   (501) staff       (20)     8033 2023-04-13 12:13:58.000000 py_shiftmanager-0.1.3/py_shiftmanager.egg-info/PKG-INFO
--rw-r--r--   0 amitnakash   (501) staff       (20)      406 2023-04-13 12:13:58.000000 py_shiftmanager-0.1.3/py_shiftmanager.egg-info/SOURCES.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)        1 2023-04-13 12:13:58.000000 py_shiftmanager-0.1.3/py_shiftmanager.egg-info/dependency_links.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       12 2023-04-13 12:13:58.000000 py_shiftmanager-0.1.3/py_shiftmanager.egg-info/requires.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       16 2023-04-13 12:13:58.000000 py_shiftmanager-0.1.3/py_shiftmanager.egg-info/top_level.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       38 2023-04-13 12:13:58.550879 py_shiftmanager-0.1.3/setup.cfg
--rw-r--r--   0 amitnakash   (501) staff       (20)      591 2023-04-13 12:06:46.000000 py_shiftmanager-0.1.3/setup.py
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-14 14:16:37.360815 py_shiftmanager-0.1.4/
+-rw-r--r--   0 amitnakash   (501) staff       (20)       17 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.4/MANIFEST.in
+-rw-r--r--   0 amitnakash   (501) staff       (20)      318 2023-04-14 14:16:37.360646 py_shiftmanager-0.1.4/PKG-INFO
+-rw-r--r--   0 amitnakash   (501) staff       (20)     8231 2023-04-14 14:15:13.000000 py_shiftmanager-0.1.4/Readme.md
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-14 14:16:37.359246 py_shiftmanager-0.1.4/py_shiftmanager/
+-rw-r--r--   0 amitnakash   (501) staff       (20)      289 2023-04-13 06:10:21.000000 py_shiftmanager-0.1.4/py_shiftmanager/__init__.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)      428 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.4/py_shiftmanager/logger.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     5300 2023-04-14 13:52:18.000000 py_shiftmanager-0.1.4/py_shiftmanager/shiftmanager_compute.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     5531 2023-04-14 13:54:57.000000 py_shiftmanager-0.1.4/py_shiftmanager/shiftmanager_io.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)      802 2023-04-14 14:07:57.000000 py_shiftmanager-0.1.4/py_shiftmanager/timeout.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     3372 2023-04-13 22:49:11.000000 py_shiftmanager-0.1.4/py_shiftmanager/worker.py
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-14 14:16:37.360332 py_shiftmanager-0.1.4/py_shiftmanager.egg-info/
+-rw-r--r--   0 amitnakash   (501) staff       (20)      318 2023-04-14 14:16:37.000000 py_shiftmanager-0.1.4/py_shiftmanager.egg-info/PKG-INFO
+-rw-r--r--   0 amitnakash   (501) staff       (20)      406 2023-04-14 14:16:37.000000 py_shiftmanager-0.1.4/py_shiftmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)        1 2023-04-14 14:16:37.000000 py_shiftmanager-0.1.4/py_shiftmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       12 2023-04-14 14:16:37.000000 py_shiftmanager-0.1.4/py_shiftmanager.egg-info/requires.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       16 2023-04-14 14:16:37.000000 py_shiftmanager-0.1.4/py_shiftmanager.egg-info/top_level.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       38 2023-04-14 14:16:37.360883 py_shiftmanager-0.1.4/setup.cfg
+-rw-r--r--   0 amitnakash   (501) staff       (20)      595 2023-04-14 14:16:30.000000 py_shiftmanager-0.1.4/setup.py
```

### Comparing `py_shiftmanager-0.1.3/PKG-INFO` & `py_shiftmanager-0.1.4/Readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,9 @@
-Metadata-Version: 2.1
-Name: py_shiftmanager
-Version: 0.1.3
-Summary: A simplified, all-in-one shop for handling multithreading/multiprocessing using a managed queue system.
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-
 # Py-ShiftManager
-#### v0.1.3
+#### v0.1.4
 
 Py-ShiftManager is a Python module that provides a managed queue environment for handling IO and computational tasks, allowing you to easily manage concurrency and multiprocessing without worrying about the details.
 
 ## Installation
 You can install Py-ShiftManager using pip:
 `pip install py-shiftmanager`
 
@@ -33,20 +25,22 @@
 #### added in v0.1.3
 * 🛠️ Improved handling of queue exceptions - a better managing solution for large incoming amount of tasks.  
 * 🛠️ Improved task submission logic.
 * 🔒 Improved encapsulation.
 * 🛠️ New method added - `configure()`; read more under *'API'* section.   
 * 🛠️ Improved concurrency and parallelism in the IO module.
 * ⌫ Deprecated methods - `queue_in_size()`, `queue_out_size()` 
+#### added in v0.1.4
+* 🛠️ Task submission now supports both *args and **kwargs. 
 
 ## Usage
 Here's an example of how to use Py-ShiftManager to handle IO tasks:  
-`from py-shiftmanager import ShiftManager_IO`.  
+`from py_shiftmanager import ShiftManager_IO`.  
 Now, lets also import *timeout_timer* wrapper:  
-`from py-shiftmanager.timeout import timeout_timer`
+`from py_shiftmanager.timeout import timeout_timer`
 
 # Create a new ShiftManager instance with 4 workers
 `manager = ShiftManager_IO(num_of_workers=4)`  
 By default *ShiftManager* objects init with these values for its attributes:
 * num_of_workers = `2`
 * daemon = `False`
 * input_q_size = `10`
@@ -63,15 +57,15 @@
 We can assign single tasks to the queue:  
 `manager.new_task(get_status, "http://www.google.com")`  
 `manager.new_task(get_status, "http://www.facebook.com")`  
 `manager.new_task(get_status, "http://www.twitter.com")`   
 Or we can submit a batch by passing a list of tuples:  
 `tasks = [(get_status, "http://www.google.com"),(get_status, "http://www.facebook.com")]`  
 `manager.new_batch(tasks)`  
-  
+
 **Note**: you can also pass in *lambda* functions.
 
 # Handle the tasks
 `manager.handle_work()`  
 *ShiftManager* spins up the workers and starts consuming tasks from the input queue.  
 Since we applied the *timeout_timer* decorator, if a task takes longer than 3 seconds - it will be terminated, but you'll still recieve a result with the task details, and that it has ran out of time.  
 
@@ -80,15 +74,15 @@
 This method sends a shut-down signal to all workers and waits for them to shut-down gracefully.
 
 **Note**: this does not interfere with retrieving results from the output queue at any time.
 
 
 And here's an example of how to use Py-ShiftManager to handle computational tasks:
 
-`from py-shiftmanager import ShiftManager_Compute`  
+`from py_shiftmanager import ShiftManager_Compute`  
 
 # Create a new ShiftManager instance with 4 workers
 `manager = ShiftManager_Compute(num_of_workers=4)`  
 But this time we'll increase the number to 5 using simple addition:  
 `manager + 1` - now *manager* is set to run 5 workers.   
 
 By default *ShiftManager_Compute* initializes with these default values for its attributes:  
@@ -125,16 +119,16 @@
 
 ## API
 
 **ShiftManager_IO**  
 `ShiftManager_IO(num_of_workers: int = 1, daemon: bool = False, input_q_size: int = 10, output_q_size: int = 15) -> None`  
 Creates a new ShiftManager instance with the specified number of workers, daemon status, input queue size and output queue size.
 
-`new_task(func: Callable, task: Any, force: bool = False) -> None`  
-Adds a new task to the input queue; you could force it if you want.
+`new_task(func: Callable, *args, force: bool = False, **kwargs) -> None`  
+Adds a new task to the input queue; accepting *args and **kwargs; you could force it if you want.
 
 `new_batch(tasks: List[tuple], force: bool = False) -> None`  
 Adds a list of tasks to the input queue; you could force it if you want.
 
 `handle_work() -> None`  
 Handles the tasks in the input queue.
 
@@ -150,19 +144,19 @@
 * `put_timeout: int` - reconfigure timeout (in seconds) for input queue task submission (default is `1` second).
 * `num_of_workers: int` - reconfigure number of workers.  
 
 **ShiftManager_Compute**  
 `ShiftManager_Compute(num_of_workers: int = 1, daemon: bool = False, input_q_size: int = 10, output_q_size: int = 15) -> None`  
 Creates a new ShiftManager instance with the specified number of workers, daemon status, input queue size and output queue size.
 
-`new_task(func: Callable, task: Any) -> None`  
-Adds a new task to the input queue.
+`new_task(func: Callable, *args, force: bool = False, **kwargs) -> None`  
+Adds a new task to the input queue; accepting *args and **kwargs; you could force it if you want.
 
-`new_batch(tasks: List[tuple]) -> None`  
-Adds a list of tasks to the input queue.
+`new_batch(tasks: List[tuple], force: bool = False) -> None`  
+Adds a list of tasks to the input queue; you could force it if you want.
 
 `handle_work() -> None`  
 Handles the tasks in the input queue.
 
 `get_results() -> List`  
 Returns the results of the completed tasks from the output queue.
 
@@ -173,8 +167,16 @@
 Allows the user to configure the following attributes by passing keyword arguments:  
 * `daemon: bool` - reconfigure workers daemon status. 
 * `put_timeout: int` - reconfigure timeout (in seconds) for input queue task submission (default is `1` second).
 * `num_of_workers: int` - reconfigure number of workers.  
 
 **timeout_timer**  
 `@timeout_timer(seconds: int = 5)`  
-A decorator that attaches a timeout counter to your methods, use it to set a time limit to tasks in seconds; `5` seconds by default.
+A decorator that attaches a timeout counter to your methods, use it to set a time limit to tasks in seconds; `5` seconds by default.  
+
+**context_manager**
+implement it using the `with` keyword:  
+`with ShiftManager_Compute() as manager:`  
+`   manager.new_task(lambda x: x**2, 4)`  
+`   manager.new_task(lambda x: x**4, 13)`  
+then get the results:  
+`results = manager.get_results()`
```

### Comparing `py_shiftmanager-0.1.3/py_shiftmanager/shiftmanager_compute.py` & `py_shiftmanager-0.1.4/py_shiftmanager/shiftmanager_compute.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,21 +76,35 @@
             self.__put_timeout = kwargs['put_timeout']
         if kwargs['num_of_workers']:
             self.__num_of_workers = kwargs['num_of_workers']
         if kwargs['daemon']:
             self.__daemon = kwargs['daemon']
             
     """ Task and queue management """
-    def new_task(self, func: Callable, *args, force: bool = False) -> NoReturn:
-        new_task = {"arrival_time": int(datetime.datetime.now().timestamp()), "func": dill.dumps(func), "args": args}
+    def new_task(self, func: Callable, *args, force: bool = False, **kwargs) -> NoReturn:
+        new_task = {"arrival_time": int(datetime.datetime.now().timestamp()), "func": dill.dumps(func), "args": args, "kwargs": kwargs}
         self.__submit_task(new_task, force)
 
-    def new_batch(self, tasks: List[tuple], force: bool = False) -> NoReturn:
+    def new_batch(self, tasks: List, force: bool = False) -> NoReturn:
         for task in tasks:
-            self.new_task(*task, force=force)
+            if len(task) == 1:
+                func = task[0]
+                args = ()
+                kwargs = {}
+            elif len(task) == 2:
+                func, arg_or_kwarg = task
+                if isinstance(arg_or_kwarg, tuple):
+                    args = arg_or_kwarg
+                    kwargs = {}
+                else:
+                    args = ()
+                    kwargs = arg_or_kwarg
+            else:
+                func, args, kwargs = task
+            self.new_task(func, *args, force=force, **kwargs)
 
     def handle_work(self) -> NoReturn:
         """ start pool without close() to enable continuous acceptance of new submitted tasks """
         self.__pool = multiprocessing.Pool(processes=self.__num_of_workers, initializer=self.__worker.work,
                                     initargs=(self.__q_in, self.__q_out))
 
     def get_results(self) -> List:
```

### Comparing `py_shiftmanager-0.1.3/py_shiftmanager/shiftmanager_io.py` & `py_shiftmanager-0.1.4/py_shiftmanager/shiftmanager_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,21 +77,35 @@
             self.__put_timeout = kwargs['put_timeout']
         if kwargs['num_of_workers']:
             self.__num_of_workers = kwargs['num_of_workers']
         if kwargs['daemon']:
             self.__daemon = kwargs['daemon']
 
     """ Task and queue management """
-    def new_task(self, func: Callable, *args, force: bool = False) -> NoReturn:
-        new_task = {"arrival_time": int(datetime.datetime.now().timestamp()), "func": dill.dumps(func), "args": args}
+    def new_task(self, func: Callable, *args, force: bool = False, **kwargs) -> NoReturn:
+        new_task = {"arrival_time": int(datetime.datetime.now().timestamp()), "func": dill.dumps(func), "args": args, "kwargs": kwargs}
         self.__submit_task(new_task, force)
 
-    def new_batch(self, tasks: List[tuple], force: bool = False) -> NoReturn:
+    def new_batch(self, tasks: List, force: bool = False) -> NoReturn:
         for task in tasks:
-            self.new_task(*task, force=force)
+            if len(task) == 1:
+                func = task[0]
+                args = ()
+                kwargs = {}
+            elif len(task) == 2:
+                func, arg_or_kwarg = task
+                if isinstance(arg_or_kwarg, tuple):
+                    args = arg_or_kwarg
+                    kwargs = {}
+                else:
+                    args = ()
+                    kwargs = arg_or_kwarg
+            else:
+                func, args, kwargs = task
+            self.new_task(func, *args, force=force, **kwargs)
 
     # def queue_in_size(self) -> int or NoReturn:
     #     try:
     #         return self.__q_in.qsize()
     #     except NotImplementedError:
     #         logger.logger.error("Input-queue .qsize() not implemented; exited gracefully.")
```

### Comparing `py_shiftmanager-0.1.3/py_shiftmanager/timeout.py` & `py_shiftmanager-0.1.4/py_shiftmanager/timeout.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 def timeout_timer(func=None, seconds=5, error_message='Task timed out.'):
     """ Timeout wrapper, sets a seconds countdown on a separate running thread with using join().
         Setting the thread daemon flag to True, so that it exits when the time runs out and program ended.
     """
     if func is None:
         return lambda f: timeout_timer(f, seconds, error_message)
 
-    def wrapper(*args):
+    def wrapper(*args, **kwargs):
         result = {"task": func.__name__, "args": args}
         def target():
-            result["result"] = func(*args)
+            result["result"] = func(*args, **kwargs)
         thread = threading.Thread(target=target)
         thread.daemon = True
         thread.start()
         thread.join(seconds)
         if thread.is_alive():
             result["error"] = error_message
         return result
```

### Comparing `py_shiftmanager-0.1.3/py_shiftmanager/worker.py` & `py_shiftmanager-0.1.4/py_shiftmanager/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,17 @@
                 if task is None:
                     qu_in.task_done()
                     self.__is_hired = False
                     break
                 self.__is_working = True
                 func = dill.loads(task['func'])
                 args = task['args']
+                kwargs = task['kwargs']
                 try:
-                    result = func(*args)
+                    result = func(*args, **kwargs)
                 except Exception as err:
                     result = {"error": err, "task": func.__name__, "args": args}
                 qu_in.task_done()
                 try:
                     lock2.acquire()
                     qu_out.put(result, timeout=1)
                 except queue.Full:
@@ -87,15 +88,16 @@
                 if isinstance(task, PoisonPill):
                     self.__is_hired = False
                     qu_in.task_done()
                     break
                 self.__is_working = True
                 func = dill.loads(task['func'])
                 args = task['args']
-                result = func(*args)
+                kwargs = task['kwargs']
+                result = func(*args, **kwargs)
                 qu_in.task_done()
                 try:
                     lock4.acquire()
                     qu_out.put(result, timeout=1)
                     lock4.release()
                 except queue.Full:
                     lock4.release()
```

### Comparing `py_shiftmanager-0.1.3/setup.py` & `py_shiftmanager-0.1.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-long_description = Path('Readme.md').read_text()
+# long_description = Path('Readme.md').read_text()
 
 setup(
     name='py_shiftmanager',
-    version='0.1.3',
+    version='0.1.4',
     description='A simplified, all-in-one shop for handling multithreading/multiprocessing using a managed queue system.',
-    long_description=long_description,
+    # long_description=long_description,
     packages=find_packages(),
     install_requires=[
         'dill==0.3.6',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

