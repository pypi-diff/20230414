# Comparing `tmp/compensating-transaction-0.0.1.tar.gz` & `tmp/compensating-transaction-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compensating-transaction-0.0.1.tar", last modified: Fri Apr 14 08:39:16 2023, max compression
+gzip compressed data, was "compensating-transaction-0.0.2.tar", last modified: Fri Apr 14 09:05:35 2023, max compression
```

## Comparing `compensating-transaction-0.0.1.tar` & `compensating-transaction-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-14 08:39:16.633850 compensating-transaction-0.0.1/
--rw-r--r--   0 ivan       (501) staff       (20)     1064 2023-04-14 07:35:53.000000 compensating-transaction-0.0.1/LICENSE
--rw-r--r--   0 ivan       (501) staff       (20)      459 2023-04-14 08:39:16.633711 compensating-transaction-0.0.1/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)     2957 2023-04-14 08:23:35.000000 compensating-transaction-0.0.1/README.md
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-14 08:39:16.632885 compensating-transaction-0.0.1/compensating_transaction/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2023-04-14 07:47:07.000000 compensating-transaction-0.0.1/compensating_transaction/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)      463 2023-04-14 07:39:08.000000 compensating-transaction-0.0.1/compensating_transaction/exceptions.py
--rw-r--r--   0 ivan       (501) staff       (20)     8459 2023-04-14 08:28:56.000000 compensating-transaction-0.0.1/compensating_transaction/transaction.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-14 08:39:16.633540 compensating-transaction-0.0.1/compensating_transaction.egg-info/
--rw-r--r--   0 ivan       (501) staff       (20)      459 2023-04-14 08:39:16.000000 compensating-transaction-0.0.1/compensating_transaction.egg-info/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)      334 2023-04-14 08:39:16.000000 compensating-transaction-0.0.1/compensating_transaction.egg-info/SOURCES.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2023-04-14 08:39:16.000000 compensating-transaction-0.0.1/compensating_transaction.egg-info/dependency_links.txt
--rw-r--r--   0 ivan       (501) staff       (20)       25 2023-04-14 08:39:16.000000 compensating-transaction-0.0.1/compensating_transaction.egg-info/top_level.txt
--rw-r--r--   0 ivan       (501) staff       (20)       38 2023-04-14 08:39:16.633887 compensating-transaction-0.0.1/setup.cfg
--rw-r--r--   0 ivan       (501) staff       (20)      747 2023-04-14 08:38:33.000000 compensating-transaction-0.0.1/setup.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-14 09:05:35.946704 compensating-transaction-0.0.2/
+-rw-r--r--   0 ivan       (501) staff       (20)     1064 2023-04-14 07:35:53.000000 compensating-transaction-0.0.2/LICENSE
+-rw-r--r--   0 ivan       (501) staff       (20)      459 2023-04-14 09:05:35.946549 compensating-transaction-0.0.2/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)     2957 2023-04-14 08:23:35.000000 compensating-transaction-0.0.2/README.md
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-14 09:05:35.945626 compensating-transaction-0.0.2/compensating_transaction/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2023-04-14 07:47:07.000000 compensating-transaction-0.0.2/compensating_transaction/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)      463 2023-04-14 07:39:08.000000 compensating-transaction-0.0.2/compensating_transaction/exceptions.py
+-rw-r--r--   0 ivan       (501) staff       (20)     8500 2023-04-14 09:02:45.000000 compensating-transaction-0.0.2/compensating_transaction/transaction.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-14 09:05:35.946364 compensating-transaction-0.0.2/compensating_transaction.egg-info/
+-rw-r--r--   0 ivan       (501) staff       (20)      459 2023-04-14 09:05:35.000000 compensating-transaction-0.0.2/compensating_transaction.egg-info/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)      334 2023-04-14 09:05:35.000000 compensating-transaction-0.0.2/compensating_transaction.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2023-04-14 09:05:35.000000 compensating-transaction-0.0.2/compensating_transaction.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan       (501) staff       (20)       25 2023-04-14 09:05:35.000000 compensating-transaction-0.0.2/compensating_transaction.egg-info/top_level.txt
+-rw-r--r--   0 ivan       (501) staff       (20)       38 2023-04-14 09:05:35.946750 compensating-transaction-0.0.2/setup.cfg
+-rw-r--r--   0 ivan       (501) staff       (20)      747 2023-04-14 09:05:09.000000 compensating-transaction-0.0.2/setup.py
```

### Comparing `compensating-transaction-0.0.1/LICENSE` & `compensating-transaction-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `compensating-transaction-0.0.1/README.md` & `compensating-transaction-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `compensating-transaction-0.0.1/compensating_transaction/transaction.py` & `compensating-transaction-0.0.2/compensating_transaction/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @dataclass
 class RollBack:
     value: typing.Optional[typing.Any] = None
 
 
 class CompensatingTransaction:
     """
-    When the function execution fails, the function execution can be rolled back, 
+    When the function execution fails, the function execution can be rolled back,
     and all previous function executions can be rolled back
     For Example:
         1. step1 -> step2 -> step3
             1). if step2 execution error:
                 rollback step1
             2). if step3 execution error:
                 rollback step2 -> rollback step1
@@ -92,15 +92,15 @@
         try:
             res = self.run_func(*self.run_args, **self.run_kwargs)
         except Exception as err:
             self._is_success = False
             if auto_rollback:
                 # After the execution fails, the upper-level operation is automatically rolled back
                 if self.rollback_exe and not isinstance(err, self.rollback_exe):
-                    # Specify the rollback exception type, only the exception 
+                    # Specify the rollback exception type, only the exception
                     # type will perform the rollback operation
                     return RollBack('ignore exe')
                 if not rollback_all:
                     self.previous_rollback()
                 else:
                     self.rollback_all()
             raise err
@@ -120,15 +120,15 @@
                 self.previous.rollback()
         return True
 
     def rollback_all(self, ignore_exe: bool = False) -> list:
         """rollback all
 
         Args:
-            ignore_exe (bool, optional): Whether to ignore the rollback exception, 
+            ignore_exe (bool, optional): Whether to ignore the rollback exception,
                 and continue to roll back other exceptions. Defaults to False.
 
         Raises:
             err: _description_
 
         Returns:
             list: [Rollback result, Rollback exception details]
@@ -164,16 +164,18 @@
                 all_previous_instance = [all_previous_instance]
             _all_previous_instance = []
             for previous_instance in all_previous_instance:
                 if (
                     previous_instance.rollback_func
                     and previous_instance._is_success is True
                 ):
-                    hash_key = f'{previous_instance.rollback_func}:{previous_instance}:'
-                            f'{previous_instance.rollback_args}:{previous_instance.rollback_kwargs}'
+                    hash_key = (
+                        f'{previous_instance.rollback_func}:{previous_instance}:'
+                        + f'{previous_instance.rollback_args}:{previous_instance.rollback_kwargs}'
+                    )
                     hash_key = hashlib.md5(hash_key.encode()).hexdigest()
                     if hash_key not in hash_set:
                         all_rollback.append(
                             {
                                 'rollback_func': previous_instance.rollback_func,
                                 'self': previous_instance,
                                 'args': previous_instance.rollback_args,
@@ -187,24 +189,24 @@
                     else:
                         _all_previous_instance.append(previous_instance.previous)
             all_previous_instance = _all_previous_instance
         return all_rollback
 
     def rollback(self):
         """rollback
-        1. If the current run_func function is successfully executed, the rollback operation is performed, 
+        1. If the current run_func function is successfully executed, the rollback operation is performed,
         otherwise it is not executed.
         2. If the current run_func function is successfully executed, execute the upper-level rollback operation,
           otherwise it will not execute.
 
         Returns:
             _type_: RollBack(True) rollback result
         """
         res = True
         if self.rollback_func and self._is_success is True:
-            # The rollback of the current operation can only be performed after the current operation is 
+            # The rollback of the current operation can only be performed after the current operation is
             # successfully executed
             self.rollback_func(*self.rollback_args, **self.rollback_kwargs)
         if self.previous:
             # When performing a rollback, automatically perform a superior rollback
             self.previous_rollback()
         return RollBack(res)
```

### Comparing `compensating-transaction-0.0.1/setup.py` & `compensating-transaction-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: rubbish
 #############################################
 
 from setuptools import find_packages, setup
 
 setup(
     name="compensating-transaction",
-    version="0.0.1",
+    version="0.0.2",
     keywords=("pip", "compensating-transaction", "atomicity"),
     description="compensating transaction",
     long_description="When the function execution fails, the function execution can be rolled back, and all previous function executions can be rolled back",
     license="MIT Licence",
     url="https://github.com/rubbish822/compensating-transaction",
     author="rubbish",
     author_email="rubbish@rubbish.com",
```

