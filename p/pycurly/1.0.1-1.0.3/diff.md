# Comparing `tmp/pycurly-1.0.1.tar.gz` & `tmp/pycurly-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycurly-1.0.1.tar", last modified: Sat Aug 15 07:50:09 2020, max compression
+gzip compressed data, was "pycurly-1.0.3.tar", last modified: Fri Apr 14 09:47:58 2023, max compression
```

## Comparing `pycurly-1.0.1.tar` & `pycurly-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 tito      (1000) tito       (100)        0 2020-08-15 07:50:09.000000 pycurly-1.0.1/
--rw-r--r--   0 tito      (1000) tito       (100)       35 2020-08-15 07:49:49.000000 pycurly-1.0.1/MANIFEST.in
--rw-r--r--   0 tito      (1000) tito       (100)      828 2020-08-15 07:50:09.000000 pycurly-1.0.1/PKG-INFO
--rw-r--r--   0 tito      (1000) tito       (100)     2066 2018-11-17 11:12:28.000000 pycurly-1.0.1/README.md
-drwxr-xr-x   0 tito      (1000) tito       (100)        0 2020-08-15 07:50:09.000000 pycurly-1.0.1/curly/
--rw-r--r--   0 tito      (1000) tito       (100)      320 2020-08-15 07:50:08.000000 pycurly-1.0.1/curly/__init__.py
--rw-r--r--   0 tito      (1000) tito       (100)   612815 2020-08-14 17:28:42.000000 pycurly-1.0.1/curly/_curly.c
--rw-r--r--   0 tito      (1000) tito       (100)    21655 2019-09-26 08:49:12.000000 pycurly-1.0.1/curly/_curly.pyx
--rw-r--r--   0 tito      (1000) tito       (100)     6365 2018-11-19 19:12:41.000000 pycurly-1.0.1/curly/_include.pxi
--rw-r--r--   0 tito      (1000) tito       (100)     3410 2019-09-26 08:49:12.000000 pycurly-1.0.1/curly/_queue.pxi
-drwxr-xr-x   0 tito      (1000) tito       (100)        0 2020-08-15 07:50:09.000000 pycurly-1.0.1/pycurly.egg-info/
--rw-r--r--   0 tito      (1000) tito       (100)      828 2020-08-15 07:50:09.000000 pycurly-1.0.1/pycurly.egg-info/PKG-INFO
--rw-r--r--   0 tito      (1000) tito       (100)      250 2020-08-15 07:50:09.000000 pycurly-1.0.1/pycurly.egg-info/SOURCES.txt
--rw-r--r--   0 tito      (1000) tito       (100)        1 2020-08-15 07:50:09.000000 pycurly-1.0.1/pycurly.egg-info/dependency_links.txt
--rw-r--r--   0 tito      (1000) tito       (100)       19 2020-08-15 07:50:09.000000 pycurly-1.0.1/pycurly.egg-info/top_level.txt
--rw-r--r--   0 tito      (1000) tito       (100)       71 2020-08-15 07:50:09.000000 pycurly-1.0.1/setup.cfg
--rw-r--r--   0 tito      (1000) tito       (100)     4901 2020-08-14 17:33:11.000000 pycurly-1.0.1/setup.py
+drwxr-xr-x   0 tito      (1000) tito      (1000)        0 2023-04-14 09:47:58.738137 pycurly-1.0.3/
+-rw-r--r--   0 tito      (1000) tito      (1000)       35 2020-08-15 07:49:49.000000 pycurly-1.0.3/MANIFEST.in
+-rw-r--r--   0 tito      (1000) tito      (1000)      698 2023-04-14 09:47:58.738137 pycurly-1.0.3/PKG-INFO
+-rw-r--r--   0 tito      (1000) tito      (1000)     2066 2018-11-17 11:12:28.000000 pycurly-1.0.3/README.md
+drwxr-xr-x   0 tito      (1000) tito      (1000)        0 2023-04-14 09:47:58.738137 pycurly-1.0.3/curly/
+-rw-r--r--   0 tito      (1000) tito      (1000)      320 2023-04-14 09:47:44.000000 pycurly-1.0.3/curly/__init__.py
+-rw-r--r--   0 tito      (1000) tito      (1000)   627055 2023-04-14 09:43:39.000000 pycurly-1.0.3/curly/_curly.c
+-rw-r--r--   0 tito      (1000) tito      (1000)    21954 2020-08-15 08:42:26.000000 pycurly-1.0.3/curly/_curly.pyx
+-rw-r--r--   0 tito      (1000) tito      (1000)     6391 2020-08-15 08:35:28.000000 pycurly-1.0.3/curly/_include.pxi
+-rw-r--r--   0 tito      (1000) tito      (1000)     3410 2020-08-15 08:38:59.000000 pycurly-1.0.3/curly/_queue.pxi
+drwxr-xr-x   0 tito      (1000) tito      (1000)        0 2023-04-14 09:47:58.738137 pycurly-1.0.3/pycurly.egg-info/
+-rw-r--r--   0 tito      (1000) tito      (1000)      698 2023-04-14 09:47:58.000000 pycurly-1.0.3/pycurly.egg-info/PKG-INFO
+-rw-r--r--   0 tito      (1000) tito      (1000)      271 2023-04-14 09:47:58.000000 pycurly-1.0.3/pycurly.egg-info/SOURCES.txt
+-rw-r--r--   0 tito      (1000) tito      (1000)        1 2023-04-14 09:47:58.000000 pycurly-1.0.3/pycurly.egg-info/dependency_links.txt
+-rw-r--r--   0 tito      (1000) tito      (1000)       19 2023-04-14 09:47:58.000000 pycurly-1.0.3/pycurly.egg-info/top_level.txt
+-rw-r--r--   0 tito      (1000) tito      (1000)       71 2023-04-14 09:47:58.738137 pycurly-1.0.3/setup.cfg
+-rw-r--r--   0 tito      (1000) tito      (1000)     5263 2023-04-14 09:46:52.000000 pycurly-1.0.3/setup.py
+drwxr-xr-x   0 tito      (1000) tito      (1000)        0 2023-04-14 09:47:58.738137 pycurly-1.0.3/tests/
+-rw-r--r--   0 tito      (1000) tito      (1000)     1113 2018-11-17 11:47:18.000000 pycurly-1.0.3/tests/test_basics.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pycurly-1.0.1/PKG-INFO` & `pycurly-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pycurly
-Version: 1.0.1
-Summary: UNKNOWN
-Home-page: UNKNOWN
-Author: UNKNOWN
-Author-email: UNKNOWN
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
+Version: 1.0.3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pycurly-1.0.1/README.md` & `pycurly-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pycurly-1.0.1/curly/_curly.c` & `pycurly-1.0.3/curly/_curly.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-/* Generated by Cython 0.29.21 */
+/* Generated by Cython 0.29.30 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/usr/include/SDL2/SDL.h",
             "/usr/include/SDL2/SDL_image.h"
         ],
         "include_dirs": [
-            "/usr/include/SDL2"
+            "/usr/include/SDL2",
+            "/usr/include/libpng16",
+            "/usr/include/webp"
         ],
         "libraries": [
             "SDL2_image",
             "SDL2",
             "curl"
         ],
         "name": "_curly",
@@ -22,23 +24,25 @@
             "curly/_queue.pxi"
         ]
     },
     "module_name": "_curly"
 }
 END: Cython Metadata */
 
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_21"
-#define CYTHON_HEX_VERSION 0x001D15F0
+#define CYTHON_ABI "0_29_30"
+#define CYTHON_HEX_VERSION 0x001D1EF0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -105,14 +109,17 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
@@ -146,14 +153,17 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
@@ -177,53 +187,64 @@
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -332,17 +353,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -448,25 +528,33 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
+  #if defined(PyUnicode_IS_READY)
   #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
                                               0 : _PyUnicode_Ready((PyObject *)(op)))
+  #else
+  #define __Pyx_PyUnicode_READY(op)       (0)
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
   #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
+  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #endif
   #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
@@ -564,18 +652,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -592,16 +680,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -731,14 +821,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -905,15 +996,15 @@
  */
 struct __pyx_t_6_curly_queue_ctx {
   __pyx_t_6_curly_queue_node *head;
   __pyx_t_6_curly_queue_node *tail;
   SDL_mutex *mutex;
 };
 
-/* "_curly.pyx":291
+/* "_curly.pyx":293
  * 
  * 
  * cdef class CurlyResult(object):             # <<<<<<<<<<<<<<
  *     """Object containing a result from a request.
  *     """
  */
 struct __pyx_obj_6_curly_CurlyResult {
@@ -1208,21 +1299,29 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyCFunctionFastCall.proto */
 #if CYTHON_FAST_PYCCALL
 static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
 #else
 #define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
@@ -1544,26 +1643,31 @@
 /* Print.proto */
 static int __Pyx_Print(PyObject*, PyObject *, int);
 #if CYTHON_COMPILING_IN_PYPY || PY_MAJOR_VERSION >= 3
 static PyObject* __pyx_print = 0;
 static PyObject* __pyx_print_kwargs = 0;
 #endif
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+/* GCCDiagnostics.proto */
+#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
 
 /* PrintOne.proto */
 static int __Pyx_PrintOne(PyObject* stream, PyObject *o);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
@@ -1614,14 +1718,15 @@
 static int __pyx_v_6_curly_dl_running;
 static int __pyx_v_6_curly_dl_stop;
 static SDL_sem *__pyx_v_6_curly_dl_sem;
 static SDL_atomic_t __pyx_v_6_curly_dl_done;
 static SDL_atomic_t __pyx_v_6_curly_dl_ready_to_process;
 static int __pyx_v_6_curly_config_num_threads;
 static int __pyx_v_6_curly_config_req_verify_peer;
+static char *__pyx_v_6_curly_config_useragent;
 static void __pyx_f_6_curly_queue_init(__pyx_t_6_curly_queue_ctx *); /*proto*/
 static int __pyx_f_6_curly_queue_append_last(__pyx_t_6_curly_queue_ctx *, void *); /*proto*/
 static int __pyx_f_6_curly_queue_append_first(__pyx_t_6_curly_queue_ctx *, void *); /*proto*/
 static void *__pyx_f_6_curly_queue_pop_first(__pyx_t_6_curly_queue_ctx *); /*proto*/
 static void __pyx_f_6_curly_dl_queue_node_free(__pyx_t_6_curly_dl_queue_data **); /*proto*/
 static size_t __pyx_f_6_curly__curl_write_data(void *, size_t, size_t, __pyx_t_6_curly_dl_queue_data *); /*proto*/
 static size_t __pyx_f_6_curly__curl_write_header(void *, size_t, size_t, __pyx_t_6_curly_dl_queue_data *); /*proto*/
@@ -1743,14 +1848,15 @@
 static const char __pyx_k_cache_dir[] = "cache_dir";
 static const char __pyx_k_configure[] = "configure";
 static const char __pyx_k_iteritems[] = "iteritems";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_rowlength[] = "rowlength";
 static const char __pyx_k_uninstall[] = "uninstall";
+static const char __pyx_k_useragent[] = "useragent";
 static const char __pyx_k_CurlyError[] = "CurlyError";
 static const char __pyx_k_kivy_clock[] = "kivy.clock";
 static const char __pyx_k_startswith[] = "startswith";
 static const char __pyx_k_unschedule[] = "unschedule";
 static const char __pyx_k_url_suffix[] = "url_suffix";
 static const char __pyx_k_CurlyResult[] = "CurlyResult";
 static const char __pyx_k_ImportError[] = "ImportError";
@@ -1768,14 +1874,15 @@
 static const char __pyx_k_download_image[] = "download_image";
 static const char __pyx_k_no_image_cache[] = "no_image_cache";
 static const char __pyx_k_ImageLoaderBase[] = "ImageLoaderBase";
 static const char __pyx_k_kivy_core_image[] = "kivy.core.image";
 static const char __pyx_k_req_verify_peer[] = "req_verify_peer";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_application_json[] = "application/json";
+static const char __pyx_k_config_useragent[] = "config_useragent";
 static const char __pyx_k_curly__curly_pyx[] = "curly/_curly.pyx";
 static const char __pyx_k_CurlyResult_url_r[] = "<CurlyResult url={!r}>";
 static const char __pyx_k_ImageLoaderMemory[] = "ImageLoaderMemory";
 static const char __pyx_k_schedule_interval[] = "schedule_interval";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_Client_Error_for_url[] = "{} Client Error: {} for url: {}";
 static const char __pyx_k_No_error_message_for[] = "No error message for {}";
@@ -1835,14 +1942,15 @@
 static PyObject *__pyx_n_s_b_string;
 static PyObject *__pyx_n_s_c_header;
 static PyObject *__pyx_n_s_cache_dir;
 static PyObject *__pyx_n_s_cache_fn;
 static PyObject *__pyx_n_s_callback;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_code;
+static PyObject *__pyx_n_s_config_useragent;
 static PyObject *__pyx_n_s_configure;
 static PyObject *__pyx_kp_s_content_type;
 static PyObject *__pyx_n_s_curl_ret;
 static PyObject *__pyx_n_s_curly;
 static PyObject *__pyx_kp_s_curly__curly_pyx;
 static PyObject *__pyx_kp_s_curly_requires_ssl_linked_otherw;
 static PyObject *__pyx_n_s_data;
@@ -1936,14 +2044,15 @@
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_uninstall;
 static PyObject *__pyx_n_s_unschedule;
 static PyObject *__pyx_n_s_url;
 static PyObject *__pyx_n_s_url_suffix;
 static PyObject *__pyx_n_s_urllib;
 static PyObject *__pyx_n_s_urllib_parse;
+static PyObject *__pyx_n_s_useragent;
 static PyObject *__pyx_n_s_utf8;
 static PyObject *__pyx_n_s_value;
 static PyObject *__pyx_n_s_version;
 static PyObject *__pyx_n_s_w;
 static PyObject *__pyx_pf_6_curly_get_info(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_6_curly_17ImageLoaderMemory___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_data, PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_6_curly_17ImageLoaderMemory_2load(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
@@ -1966,15 +2075,15 @@
 static PyObject *__pyx_pf_6_curly_11CurlyResult_16__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6_curly_CurlyResult *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_6_curly_2request(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_url, PyObject *__pyx_v_callback, PyObject *__pyx_v_headers, PyObject *__pyx_v_method, PyObject *__pyx_v_params, PyObject *__pyx_v_data, PyObject *__pyx_v_json, PyObject *__pyx_v_auth, PyObject *__pyx_v_cache_fn, PyObject *__pyx_v_preload_image, PyObject *__pyx_v_priority, PyObject *__pyx_v_no_image_cache); /* proto */
 static PyObject *__pyx_pf_6_curly_4download_image(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_6_curly_6process(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_args); /* proto */
 static PyObject *__pyx_pf_6_curly_8install(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_6_curly_10uninstall(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_6_curly_12stop(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_6_curly_14configure(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_num_threads, PyObject *__pyx_v_req_verify_peer); /* proto */
+static PyObject *__pyx_pf_6_curly_14configure(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_num_threads, PyObject *__pyx_v_req_verify_peer, PyObject *__pyx_v_useragent); /* proto */
 static PyObject *__pyx_tp_new_6_curly_CurlyResult(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyBytes_Type_split = {0, &__pyx_n_s_split, 0, 0, 0};
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_3;
 static PyObject *__pyx_int_4;
 static PyObject *__pyx_int_400;
@@ -3014,15 +3123,15 @@
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "_curly.pyx":46
+/* "_curly.pyx":47
  * 
  * 
  * cdef size_t _curl_write_data(void *ptr, size_t size, size_t nmemb, dl_queue_data *data) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t index = data.size
  */
 
@@ -3030,243 +3139,243 @@
   size_t __pyx_v_index;
   size_t __pyx_v_n;
   char *__pyx_v_tmp;
   size_t __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
 
-  /* "_curly.pyx":48
+  /* "_curly.pyx":49
  * cdef size_t _curl_write_data(void *ptr, size_t size, size_t nmemb, dl_queue_data *data) nogil:
  *     cdef:
  *         size_t index = data.size             # <<<<<<<<<<<<<<
  *         size_t n = (size * nmemb)
  *         char* tmp
  */
   __pyx_t_1 = __pyx_v_data->size;
   __pyx_v_index = __pyx_t_1;
 
-  /* "_curly.pyx":49
+  /* "_curly.pyx":50
  *     cdef:
  *         size_t index = data.size
  *         size_t n = (size * nmemb)             # <<<<<<<<<<<<<<
  *         char* tmp
  *     data.size += (size * nmemb)
  */
   __pyx_v_n = (__pyx_v_size * __pyx_v_nmemb);
 
-  /* "_curly.pyx":51
+  /* "_curly.pyx":52
  *         size_t n = (size * nmemb)
  *         char* tmp
  *     data.size += (size * nmemb)             # <<<<<<<<<<<<<<
  *     tmp = <char *>realloc(data.data, data.size + 1)
  * 
  */
   __pyx_v_data->size = (__pyx_v_data->size + (__pyx_v_size * __pyx_v_nmemb));
 
-  /* "_curly.pyx":52
+  /* "_curly.pyx":53
  *         char* tmp
  *     data.size += (size * nmemb)
  *     tmp = <char *>realloc(data.data, data.size + 1)             # <<<<<<<<<<<<<<
  * 
  *     if tmp != NULL:
  */
   __pyx_v_tmp = ((char *)realloc(__pyx_v_data->data, (__pyx_v_data->size + 1)));
 
-  /* "_curly.pyx":54
+  /* "_curly.pyx":55
  *     tmp = <char *>realloc(data.data, data.size + 1)
  * 
  *     if tmp != NULL:             # <<<<<<<<<<<<<<
  *         data.data = tmp
  *     else:
  */
   __pyx_t_2 = ((__pyx_v_tmp != NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "_curly.pyx":55
+    /* "_curly.pyx":56
  * 
  *     if tmp != NULL:
  *         data.data = tmp             # <<<<<<<<<<<<<<
  *     else:
  *         if data.data != NULL:
  */
     __pyx_v_data->data = __pyx_v_tmp;
 
-    /* "_curly.pyx":54
+    /* "_curly.pyx":55
  *     tmp = <char *>realloc(data.data, data.size + 1)
  * 
  *     if tmp != NULL:             # <<<<<<<<<<<<<<
  *         data.data = tmp
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "_curly.pyx":57
+  /* "_curly.pyx":58
  *         data.data = tmp
  *     else:
  *         if data.data != NULL:             # <<<<<<<<<<<<<<
  *             free(data.data)
  *         return 0
  */
   /*else*/ {
     __pyx_t_2 = ((__pyx_v_data->data != NULL) != 0);
     if (__pyx_t_2) {
 
-      /* "_curly.pyx":58
+      /* "_curly.pyx":59
  *     else:
  *         if data.data != NULL:
  *             free(data.data)             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
       free(__pyx_v_data->data);
 
-      /* "_curly.pyx":57
+      /* "_curly.pyx":58
  *         data.data = tmp
  *     else:
  *         if data.data != NULL:             # <<<<<<<<<<<<<<
  *             free(data.data)
  *         return 0
  */
     }
 
-    /* "_curly.pyx":59
+    /* "_curly.pyx":60
  *         if data.data != NULL:
  *             free(data.data)
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     memcpy((data.data + index), ptr, n)
  */
     __pyx_r = 0;
     goto __pyx_L0;
   }
   __pyx_L3:;
 
-  /* "_curly.pyx":61
+  /* "_curly.pyx":62
  *         return 0
  * 
  *     memcpy((data.data + index), ptr, n)             # <<<<<<<<<<<<<<
  *     data.data[data.size] = '\0'
  *     return size * nmemb
  */
   (void)(memcpy((__pyx_v_data->data + __pyx_v_index), __pyx_v_ptr, __pyx_v_n));
 
-  /* "_curly.pyx":62
+  /* "_curly.pyx":63
  * 
  *     memcpy((data.data + index), ptr, n)
  *     data.data[data.size] = '\0'             # <<<<<<<<<<<<<<
  *     return size * nmemb
  * 
  */
   (__pyx_v_data->data[__pyx_v_data->size]) = '\x00';
 
-  /* "_curly.pyx":63
+  /* "_curly.pyx":64
  *     memcpy((data.data + index), ptr, n)
  *     data.data[data.size] = '\0'
  *     return size * nmemb             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = (__pyx_v_size * __pyx_v_nmemb);
   goto __pyx_L0;
 
-  /* "_curly.pyx":46
+  /* "_curly.pyx":47
  * 
  * 
  * cdef size_t _curl_write_data(void *ptr, size_t size, size_t nmemb, dl_queue_data *data) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t index = data.size
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "_curly.pyx":66
+/* "_curly.pyx":67
  * 
  * 
  * cdef size_t _curl_write_header(void *ptr, size_t size, size_t nmemb, dl_queue_data *data) nogil:             # <<<<<<<<<<<<<<
  *     cdef char *tmp
  * 
  */
 
 static size_t __pyx_f_6_curly__curl_write_header(void *__pyx_v_ptr, size_t __pyx_v_size, size_t __pyx_v_nmemb, __pyx_t_6_curly_dl_queue_data *__pyx_v_data) {
   char *__pyx_v_tmp;
   size_t __pyx_r;
 
-  /* "_curly.pyx":69
+  /* "_curly.pyx":70
  *     cdef char *tmp
  * 
  *     tmp = <char *>malloc(size * nmemb + 1)             # <<<<<<<<<<<<<<
  *     memcpy(tmp, ptr, size * nmemb)
  *     tmp[size * nmemb] = '\0'
  */
   __pyx_v_tmp = ((char *)malloc(((__pyx_v_size * __pyx_v_nmemb) + 1)));
 
-  /* "_curly.pyx":70
+  /* "_curly.pyx":71
  * 
  *     tmp = <char *>malloc(size * nmemb + 1)
  *     memcpy(tmp, ptr, size * nmemb)             # <<<<<<<<<<<<<<
  *     tmp[size * nmemb] = '\0'
  * 
  */
   (void)(memcpy(__pyx_v_tmp, __pyx_v_ptr, (__pyx_v_size * __pyx_v_nmemb)));
 
-  /* "_curly.pyx":71
+  /* "_curly.pyx":72
  *     tmp = <char *>malloc(size * nmemb + 1)
  *     memcpy(tmp, ptr, size * nmemb)
  *     tmp[size * nmemb] = '\0'             # <<<<<<<<<<<<<<
  * 
  *     data.resp_headers = curl_slist_append(
  */
   (__pyx_v_tmp[(__pyx_v_size * __pyx_v_nmemb)]) = '\x00';
 
-  /* "_curly.pyx":73
+  /* "_curly.pyx":74
  *     tmp[size * nmemb] = '\0'
  * 
  *     data.resp_headers = curl_slist_append(             # <<<<<<<<<<<<<<
  *         data.resp_headers, tmp)
  * 
  */
   __pyx_v_data->resp_headers = curl_slist_append(__pyx_v_data->resp_headers, __pyx_v_tmp);
 
-  /* "_curly.pyx":76
+  /* "_curly.pyx":77
  *         data.resp_headers, tmp)
  * 
  *     free(tmp)             # <<<<<<<<<<<<<<
  *     return size * nmemb
  * 
  */
   free(__pyx_v_tmp);
 
-  /* "_curly.pyx":77
+  /* "_curly.pyx":78
  * 
  *     free(tmp)
  *     return size * nmemb             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = (__pyx_v_size * __pyx_v_nmemb);
   goto __pyx_L0;
 
-  /* "_curly.pyx":66
+  /* "_curly.pyx":67
  * 
  * 
  * cdef size_t _curl_write_header(void *ptr, size_t size, size_t nmemb, dl_queue_data *data) nogil:             # <<<<<<<<<<<<<<
  *     cdef char *tmp
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "_curly.pyx":80
+/* "_curly.pyx":81
  * 
  * 
  * cdef int dl_run_job(void *arg) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         dl_queue_data *data
  */
 
@@ -3277,15 +3386,15 @@
   int __pyx_v_require_download;
   FILE *__pyx_v_fp;
   int __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
 
   /* "_curly.pyx":89
- * 
+ *         FILE *fp
  * 
  *     curl = curl_easy_init()             # <<<<<<<<<<<<<<
  *     if not curl:
  *         return -1
  */
   __pyx_v_curl = curl_easy_init();
 
@@ -3513,689 +3622,717 @@
         goto __pyx_L11;
       }
 
       /* "_curly.pyx":116
  *                 curl_easy_setopt(curl, CURLOPT_HTTPHEADER, data.headers)
  *             else:
  *                 curl_easy_setopt(curl, CURLOPT_HTTPHEADER, NULL)             # <<<<<<<<<<<<<<
- *             if data.auth_userpwd != NULL:
- *                 curl_easy_setopt(curl, CURLOPT_HTTPAUTH, CURLAUTH_ANY)
+ *             if config_useragent != NULL:
+ *                 curl_easy_setopt(curl, CURLOPT_USERAGENT, config_useragent)
  */
       /*else*/ {
         (void)(curl_easy_setopt(__pyx_v_curl, CURLOPT_HTTPHEADER, NULL));
       }
       __pyx_L11:;
 
       /* "_curly.pyx":117
  *             else:
  *                 curl_easy_setopt(curl, CURLOPT_HTTPHEADER, NULL)
+ *             if config_useragent != NULL:             # <<<<<<<<<<<<<<
+ *                 curl_easy_setopt(curl, CURLOPT_USERAGENT, config_useragent)
+ *             if data.auth_userpwd != NULL:
+ */
+      __pyx_t_1 = ((__pyx_v_6_curly_config_useragent != NULL) != 0);
+      if (__pyx_t_1) {
+
+        /* "_curly.pyx":118
+ *                 curl_easy_setopt(curl, CURLOPT_HTTPHEADER, NULL)
+ *             if config_useragent != NULL:
+ *                 curl_easy_setopt(curl, CURLOPT_USERAGENT, config_useragent)             # <<<<<<<<<<<<<<
+ *             if data.auth_userpwd != NULL:
+ *                 curl_easy_setopt(curl, CURLOPT_HTTPAUTH, CURLAUTH_ANY)
+ */
+        (void)(curl_easy_setopt(__pyx_v_curl, CURLOPT_USERAGENT, __pyx_v_6_curly_config_useragent));
+
+        /* "_curly.pyx":117
+ *             else:
+ *                 curl_easy_setopt(curl, CURLOPT_HTTPHEADER, NULL)
+ *             if config_useragent != NULL:             # <<<<<<<<<<<<<<
+ *                 curl_easy_setopt(curl, CURLOPT_USERAGENT, config_useragent)
+ *             if data.auth_userpwd != NULL:
+ */
+      }
+
+      /* "_curly.pyx":119
+ *             if config_useragent != NULL:
+ *                 curl_easy_setopt(curl, CURLOPT_USERAGENT, config_useragent)
  *             if data.auth_userpwd != NULL:             # <<<<<<<<<<<<<<
  *                 curl_easy_setopt(curl, CURLOPT_HTTPAUTH, CURLAUTH_ANY)
  *                 curl_easy_setopt(curl, CURLOPT_USERPWD, data.auth_userpwd)
  */
       __pyx_t_1 = ((__pyx_v_data->auth_userpwd != NULL) != 0);
       if (__pyx_t_1) {
 
-        /* "_curly.pyx":118
- *                 curl_easy_setopt(curl, CURLOPT_HTTPHEADER, NULL)
+        /* "_curly.pyx":120
+ *                 curl_easy_setopt(curl, CURLOPT_USERAGENT, config_useragent)
  *             if data.auth_userpwd != NULL:
  *                 curl_easy_setopt(curl, CURLOPT_HTTPAUTH, CURLAUTH_ANY)             # <<<<<<<<<<<<<<
  *                 curl_easy_setopt(curl, CURLOPT_USERPWD, data.auth_userpwd)
  *             if data.postdata != NULL:
  */
         (void)(curl_easy_setopt(__pyx_v_curl, CURLOPT_HTTPAUTH, CURLAUTH_ANY));
 
-        /* "_curly.pyx":119
+        /* "_curly.pyx":121
  *             if data.auth_userpwd != NULL:
  *                 curl_easy_setopt(curl, CURLOPT_HTTPAUTH, CURLAUTH_ANY)
  *                 curl_easy_setopt(curl, CURLOPT_USERPWD, data.auth_userpwd)             # <<<<<<<<<<<<<<
  *             if data.postdata != NULL:
  *                 curl_easy_setopt(curl, CURLOPT_POSTFIELDS, data.postdata)
  */
         (void)(curl_easy_setopt(__pyx_v_curl, CURLOPT_USERPWD, __pyx_v_data->auth_userpwd));
 
-        /* "_curly.pyx":117
- *             else:
- *                 curl_easy_setopt(curl, CURLOPT_HTTPHEADER, NULL)
+        /* "_curly.pyx":119
+ *             if config_useragent != NULL:
+ *                 curl_easy_setopt(curl, CURLOPT_USERAGENT, config_useragent)
  *             if data.auth_userpwd != NULL:             # <<<<<<<<<<<<<<
  *                 curl_easy_setopt(curl, CURLOPT_HTTPAUTH, CURLAUTH_ANY)
  *                 curl_easy_setopt(curl, CURLOPT_USERPWD, data.auth_userpwd)
  */
       }
 
-      /* "_curly.pyx":120
+      /* "_curly.pyx":122
  *                 curl_easy_setopt(curl, CURLOPT_HTTPAUTH, CURLAUTH_ANY)
  *                 curl_easy_setopt(curl, CURLOPT_USERPWD, data.auth_userpwd)
  *             if data.postdata != NULL:             # <<<<<<<<<<<<<<
  *                 curl_easy_setopt(curl, CURLOPT_POSTFIELDS, data.postdata)
  *                 curl_easy_setopt(curl, CURLOPT_POSTFIELDSIZE, strlen(data.postdata))
  */
       __pyx_t_1 = ((__pyx_v_data->postdata != NULL) != 0);
       if (__pyx_t_1) {
 
-        /* "_curly.pyx":121
+        /* "_curly.pyx":123
  *                 curl_easy_setopt(curl, CURLOPT_USERPWD, data.auth_userpwd)
  *             if data.postdata != NULL:
  *                 curl_easy_setopt(curl, CURLOPT_POSTFIELDS, data.postdata)             # <<<<<<<<<<<<<<
  *                 curl_easy_setopt(curl, CURLOPT_POSTFIELDSIZE, strlen(data.postdata))
  *             if strncmp(data.method, "GET", 3) == 0:
  */
         (void)(curl_easy_setopt(__pyx_v_curl, CURLOPT_POSTFIELDS, __pyx_v_data->postdata));
 
-        /* "_curly.pyx":122
+        /* "_curly.pyx":124
  *             if data.postdata != NULL:
  *                 curl_easy_setopt(curl, CURLOPT_POSTFIELDS, data.postdata)
  *                 curl_easy_setopt(curl, CURLOPT_POSTFIELDSIZE, strlen(data.postdata))             # <<<<<<<<<<<<<<
  *             if strncmp(data.method, "GET", 3) == 0:
  *                 curl_easy_setopt(curl, CURLOPT_HTTPGET, 1)
  */
         (void)(curl_easy_setopt(__pyx_v_curl, CURLOPT_POSTFIELDSIZE, strlen(__pyx_v_data->postdata)));
 
-        /* "_curly.pyx":120
+        /* "_curly.pyx":122
  *                 curl_easy_setopt(curl, CURLOPT_HTTPAUTH, CURLAUTH_ANY)
  *                 curl_easy_setopt(curl, CURLOPT_USERPWD, data.auth_userpwd)
  *             if data.postdata != NULL:             # <<<<<<<<<<<<<<
  *                 curl_easy_setopt(curl, CURLOPT_POSTFIELDS, data.postdata)
  *                 curl_easy_setopt(curl, CURLOPT_POSTFIELDSIZE, strlen(data.postdata))
  */
       }
 
-      /* "_curly.pyx":123
+      /* "_curly.pyx":125
  *                 curl_easy_setopt(curl, CURLOPT_POSTFIELDS, data.postdata)
  *                 curl_easy_setopt(curl, CURLOPT_POSTFIELDSIZE, strlen(data.postdata))
  *             if strncmp(data.method, "GET", 3) == 0:             # <<<<<<<<<<<<<<
  *                 curl_easy_setopt(curl, CURLOPT_HTTPGET, 1)
  *             elif strncmp(data.method, "POST", 4) == 0:
  */
       __pyx_t_1 = ((strncmp(__pyx_v_data->method, ((char const *)"GET"), 3) == 0) != 0);
       if (__pyx_t_1) {
 
-        /* "_curly.pyx":124
+        /* "_curly.pyx":126
  *                 curl_easy_setopt(curl, CURLOPT_POSTFIELDSIZE, strlen(data.postdata))
  *             if strncmp(data.method, "GET", 3) == 0:
  *                 curl_easy_setopt(curl, CURLOPT_HTTPGET, 1)             # <<<<<<<<<<<<<<
  *             elif strncmp(data.method, "POST", 4) == 0:
  *                 curl_easy_setopt(curl, CURLOPT_HTTPPOST, 1)
  */
         (void)(curl_easy_setopt(__pyx_v_curl, CURLOPT_HTTPGET, 1));
 
-        /* "_curly.pyx":123
+        /* "_curly.pyx":125
  *                 curl_easy_setopt(curl, CURLOPT_POSTFIELDS, data.postdata)
  *                 curl_easy_setopt(curl, CURLOPT_POSTFIELDSIZE, strlen(data.postdata))
  *             if strncmp(data.method, "GET", 3) == 0:             # <<<<<<<<<<<<<<
  *                 curl_easy_setopt(curl, CURLOPT_HTTPGET, 1)
  *             elif strncmp(data.method, "POST", 4) == 0:
  */
-        goto __pyx_L14;
+        goto __pyx_L15;
       }
 
-      /* "_curly.pyx":125
+      /* "_curly.pyx":127
  *             if strncmp(data.method, "GET", 3) == 0:
  *                 curl_easy_setopt(curl, CURLOPT_HTTPGET, 1)
  *             elif strncmp(data.method, "POST", 4) == 0:             # <<<<<<<<<<<<<<
  *                 curl_easy_setopt(curl, CURLOPT_HTTPPOST, 1)
  *             else:
  */
       __pyx_t_1 = ((strncmp(__pyx_v_data->method, ((char const *)"POST"), 4) == 0) != 0);
       if (__pyx_t_1) {
 
-        /* "_curly.pyx":126
+        /* "_curly.pyx":128
  *                 curl_easy_setopt(curl, CURLOPT_HTTPGET, 1)
  *             elif strncmp(data.method, "POST", 4) == 0:
  *                 curl_easy_setopt(curl, CURLOPT_HTTPPOST, 1)             # <<<<<<<<<<<<<<
  *             else:
  *                 curl_easy_setopt(curl, CURLOPT_CUSTOMREQUEST, data.method)
  */
         (void)(curl_easy_setopt(__pyx_v_curl, CURLOPT_HTTPPOST, 1));
 
-        /* "_curly.pyx":125
+        /* "_curly.pyx":127
  *             if strncmp(data.method, "GET", 3) == 0:
  *                 curl_easy_setopt(curl, CURLOPT_HTTPGET, 1)
  *             elif strncmp(data.method, "POST", 4) == 0:             # <<<<<<<<<<<<<<
  *                 curl_easy_setopt(curl, CURLOPT_HTTPPOST, 1)
  *             else:
  */
-        goto __pyx_L14;
+        goto __pyx_L15;
       }
 
-      /* "_curly.pyx":128
+      /* "_curly.pyx":130
  *                 curl_easy_setopt(curl, CURLOPT_HTTPPOST, 1)
  *             else:
  *                 curl_easy_setopt(curl, CURLOPT_CUSTOMREQUEST, data.method)             # <<<<<<<<<<<<<<
  *             curl_easy_setopt(curl, CURLOPT_SSL_VERIFYPEER, <void *><long>config_req_verify_peer)
  *             data.curl_ret = curl_easy_perform(curl)
  */
       /*else*/ {
         (void)(curl_easy_setopt(__pyx_v_curl, CURLOPT_CUSTOMREQUEST, __pyx_v_data->method));
       }
-      __pyx_L14:;
+      __pyx_L15:;
 
-      /* "_curly.pyx":129
+      /* "_curly.pyx":131
  *             else:
  *                 curl_easy_setopt(curl, CURLOPT_CUSTOMREQUEST, data.method)
  *             curl_easy_setopt(curl, CURLOPT_SSL_VERIFYPEER, <void *><long>config_req_verify_peer)             # <<<<<<<<<<<<<<
  *             data.curl_ret = curl_easy_perform(curl)
  * 
  */
       (void)(curl_easy_setopt(__pyx_v_curl, CURLOPT_SSL_VERIFYPEER, ((void *)((long)__pyx_v_6_curly_config_req_verify_peer))));
 
-      /* "_curly.pyx":130
+      /* "_curly.pyx":132
  *                 curl_easy_setopt(curl, CURLOPT_CUSTOMREQUEST, data.method)
  *             curl_easy_setopt(curl, CURLOPT_SSL_VERIFYPEER, <void *><long>config_req_verify_peer)
  *             data.curl_ret = curl_easy_perform(curl)             # <<<<<<<<<<<<<<
  * 
  *             if data.curl_ret != 0:
  */
       __pyx_v_data->curl_ret = curl_easy_perform(__pyx_v_curl);
 
-      /* "_curly.pyx":132
+      /* "_curly.pyx":134
  *             data.curl_ret = curl_easy_perform(curl)
  * 
  *             if data.curl_ret != 0:             # <<<<<<<<<<<<<<
  *                 # if the request failed for any reason,
  *                 # avoid any sort of image preloading
  */
       __pyx_t_1 = ((__pyx_v_data->curl_ret != 0) != 0);
       if (__pyx_t_1) {
 
-        /* "_curly.pyx":135
+        /* "_curly.pyx":137
  *                 # if the request failed for any reason,
  *                 # avoid any sort of image preloading
  *                 data.preload_image = 0             # <<<<<<<<<<<<<<
  * 
  *             elif data.cache_fn != NULL and data.size > 0:
  */
         __pyx_v_data->preload_image = 0;
 
-        /* "_curly.pyx":132
+        /* "_curly.pyx":134
  *             data.curl_ret = curl_easy_perform(curl)
  * 
  *             if data.curl_ret != 0:             # <<<<<<<<<<<<<<
  *                 # if the request failed for any reason,
  *                 # avoid any sort of image preloading
  */
-        goto __pyx_L15;
+        goto __pyx_L16;
       }
 
-      /* "_curly.pyx":137
+      /* "_curly.pyx":139
  *                 data.preload_image = 0
  * 
  *             elif data.cache_fn != NULL and data.size > 0:             # <<<<<<<<<<<<<<
  *                 fp = fopen(data.cache_fn, "wb")
  *                 fwrite(data.data, data.size, 1, fp)
  */
       __pyx_t_2 = ((__pyx_v_data->cache_fn != NULL) != 0);
       if (__pyx_t_2) {
       } else {
         __pyx_t_1 = __pyx_t_2;
-        goto __pyx_L16_bool_binop_done;
+        goto __pyx_L17_bool_binop_done;
       }
       __pyx_t_2 = ((__pyx_v_data->size > 0) != 0);
       __pyx_t_1 = __pyx_t_2;
-      __pyx_L16_bool_binop_done:;
+      __pyx_L17_bool_binop_done:;
       if (__pyx_t_1) {
 
-        /* "_curly.pyx":138
+        /* "_curly.pyx":140
  * 
  *             elif data.cache_fn != NULL and data.size > 0:
  *                 fp = fopen(data.cache_fn, "wb")             # <<<<<<<<<<<<<<
  *                 fwrite(data.data, data.size, 1, fp)
  *                 fclose(fp)
  */
         __pyx_v_fp = fopen(__pyx_v_data->cache_fn, ((char const *)"wb"));
 
-        /* "_curly.pyx":139
+        /* "_curly.pyx":141
  *             elif data.cache_fn != NULL and data.size > 0:
  *                 fp = fopen(data.cache_fn, "wb")
  *                 fwrite(data.data, data.size, 1, fp)             # <<<<<<<<<<<<<<
  *                 fclose(fp)
  * 
  */
         (void)(fwrite(__pyx_v_data->data, __pyx_v_data->size, 1, __pyx_v_fp));
 
-        /* "_curly.pyx":140
+        /* "_curly.pyx":142
  *                 fp = fopen(data.cache_fn, "wb")
  *                 fwrite(data.data, data.size, 1, fp)
  *                 fclose(fp)             # <<<<<<<<<<<<<<
  * 
  *         # dynamically load the image too ?
  */
         (void)(fclose(__pyx_v_fp));
 
-        /* "_curly.pyx":137
+        /* "_curly.pyx":139
  *                 data.preload_image = 0
  * 
  *             elif data.cache_fn != NULL and data.size > 0:             # <<<<<<<<<<<<<<
  *                 fp = fopen(data.cache_fn, "wb")
  *                 fwrite(data.data, data.size, 1, fp)
  */
       }
-      __pyx_L15:;
+      __pyx_L16:;
 
       /* "_curly.pyx":104
  *             require_download = 0
  * 
  *         if require_download:             # <<<<<<<<<<<<<<
  *             # download from url
  *             curl_easy_setopt(curl, CURLOPT_URL, data.url)
  */
     }
 
-    /* "_curly.pyx":143
+    /* "_curly.pyx":145
  * 
  *         # dynamically load the image too ?
  *         if data.preload_image:             # <<<<<<<<<<<<<<
  *             rw = NULL
  *             if data.size > 0:
  */
     __pyx_t_1 = (__pyx_v_data->preload_image != 0);
     if (__pyx_t_1) {
 
-      /* "_curly.pyx":144
+      /* "_curly.pyx":146
  *         # dynamically load the image too ?
  *         if data.preload_image:
  *             rw = NULL             # <<<<<<<<<<<<<<
  *             if data.size > 0:
  *                 rw = SDL_RWFromMem(data.data, data.size)
  */
       __pyx_v_rw = NULL;
 
-      /* "_curly.pyx":145
+      /* "_curly.pyx":147
  *         if data.preload_image:
  *             rw = NULL
  *             if data.size > 0:             # <<<<<<<<<<<<<<
  *                 rw = SDL_RWFromMem(data.data, data.size)
  *             elif data.cache_fn != NULL:
  */
       __pyx_t_1 = ((__pyx_v_data->size > 0) != 0);
       if (__pyx_t_1) {
 
-        /* "_curly.pyx":146
+        /* "_curly.pyx":148
  *             rw = NULL
  *             if data.size > 0:
  *                 rw = SDL_RWFromMem(data.data, data.size)             # <<<<<<<<<<<<<<
  *             elif data.cache_fn != NULL:
  *                 rw = SDL_RWFromFile(data.cache_fn, "rb")
  */
         __pyx_v_rw = SDL_RWFromMem(__pyx_v_data->data, __pyx_v_data->size);
 
-        /* "_curly.pyx":145
+        /* "_curly.pyx":147
  *         if data.preload_image:
  *             rw = NULL
  *             if data.size > 0:             # <<<<<<<<<<<<<<
  *                 rw = SDL_RWFromMem(data.data, data.size)
  *             elif data.cache_fn != NULL:
  */
-        goto __pyx_L19;
+        goto __pyx_L20;
       }
 
-      /* "_curly.pyx":147
+      /* "_curly.pyx":149
  *             if data.size > 0:
  *                 rw = SDL_RWFromMem(data.data, data.size)
  *             elif data.cache_fn != NULL:             # <<<<<<<<<<<<<<
  *                 rw = SDL_RWFromFile(data.cache_fn, "rb")
  *             if rw:
  */
       __pyx_t_1 = ((__pyx_v_data->cache_fn != NULL) != 0);
       if (__pyx_t_1) {
 
-        /* "_curly.pyx":148
+        /* "_curly.pyx":150
  *                 rw = SDL_RWFromMem(data.data, data.size)
  *             elif data.cache_fn != NULL:
  *                 rw = SDL_RWFromFile(data.cache_fn, "rb")             # <<<<<<<<<<<<<<
  *             if rw:
  *                 data.image = IMG_Load_RW(rw, 1)
  */
         __pyx_v_rw = SDL_RWFromFile(__pyx_v_data->cache_fn, ((char *)"rb"));
 
-        /* "_curly.pyx":147
+        /* "_curly.pyx":149
  *             if data.size > 0:
  *                 rw = SDL_RWFromMem(data.data, data.size)
  *             elif data.cache_fn != NULL:             # <<<<<<<<<<<<<<
  *                 rw = SDL_RWFromFile(data.cache_fn, "rb")
  *             if rw:
  */
       }
-      __pyx_L19:;
+      __pyx_L20:;
 
-      /* "_curly.pyx":149
+      /* "_curly.pyx":151
  *             elif data.cache_fn != NULL:
  *                 rw = SDL_RWFromFile(data.cache_fn, "rb")
  *             if rw:             # <<<<<<<<<<<<<<
  *                 data.image = IMG_Load_RW(rw, 1)
  *                 if data.image == NULL:
  */
       __pyx_t_1 = (__pyx_v_rw != 0);
       if (__pyx_t_1) {
 
-        /* "_curly.pyx":150
+        /* "_curly.pyx":152
  *                 rw = SDL_RWFromFile(data.cache_fn, "rb")
  *             if rw:
  *                 data.image = IMG_Load_RW(rw, 1)             # <<<<<<<<<<<<<<
  *                 if data.image == NULL:
  *                     data.image_error = <char *>IMG_GetError()
  */
         __pyx_v_data->image = IMG_Load_RW(__pyx_v_rw, 1);
 
-        /* "_curly.pyx":151
+        /* "_curly.pyx":153
  *             if rw:
  *                 data.image = IMG_Load_RW(rw, 1)
  *                 if data.image == NULL:             # <<<<<<<<<<<<<<
  *                     data.image_error = <char *>IMG_GetError()
  *                 if data.data != NULL:
  */
         __pyx_t_1 = ((__pyx_v_data->image == NULL) != 0);
         if (__pyx_t_1) {
 
-          /* "_curly.pyx":152
+          /* "_curly.pyx":154
  *                 data.image = IMG_Load_RW(rw, 1)
  *                 if data.image == NULL:
  *                     data.image_error = <char *>IMG_GetError()             # <<<<<<<<<<<<<<
  *                 if data.data != NULL:
  *                     free(data.data)
  */
           __pyx_v_data->image_error = ((char *)IMG_GetError());
 
-          /* "_curly.pyx":151
+          /* "_curly.pyx":153
  *             if rw:
  *                 data.image = IMG_Load_RW(rw, 1)
  *                 if data.image == NULL:             # <<<<<<<<<<<<<<
  *                     data.image_error = <char *>IMG_GetError()
  *                 if data.data != NULL:
  */
         }
 
-        /* "_curly.pyx":153
+        /* "_curly.pyx":155
  *                 if data.image == NULL:
  *                     data.image_error = <char *>IMG_GetError()
  *                 if data.data != NULL:             # <<<<<<<<<<<<<<
  *                     free(data.data)
  *                 data.data = NULL
  */
         __pyx_t_1 = ((__pyx_v_data->data != NULL) != 0);
         if (__pyx_t_1) {
 
-          /* "_curly.pyx":154
+          /* "_curly.pyx":156
  *                     data.image_error = <char *>IMG_GetError()
  *                 if data.data != NULL:
  *                     free(data.data)             # <<<<<<<<<<<<<<
  *                 data.data = NULL
  * 
  */
           free(__pyx_v_data->data);
 
-          /* "_curly.pyx":153
+          /* "_curly.pyx":155
  *                 if data.image == NULL:
  *                     data.image_error = <char *>IMG_GetError()
  *                 if data.data != NULL:             # <<<<<<<<<<<<<<
  *                     free(data.data)
  *                 data.data = NULL
  */
         }
 
-        /* "_curly.pyx":155
+        /* "_curly.pyx":157
  *                 if data.data != NULL:
  *                     free(data.data)
  *                 data.data = NULL             # <<<<<<<<<<<<<<
  * 
  *         queue_append_last(&ctx_result, data)
  */
         __pyx_v_data->data = NULL;
 
-        /* "_curly.pyx":149
+        /* "_curly.pyx":151
  *             elif data.cache_fn != NULL:
  *                 rw = SDL_RWFromFile(data.cache_fn, "rb")
  *             if rw:             # <<<<<<<<<<<<<<
  *                 data.image = IMG_Load_RW(rw, 1)
  *                 if data.image == NULL:
  */
       }
 
-      /* "_curly.pyx":143
+      /* "_curly.pyx":145
  * 
  *         # dynamically load the image too ?
  *         if data.preload_image:             # <<<<<<<<<<<<<<
  *             rw = NULL
  *             if data.size > 0:
  */
     }
 
-    /* "_curly.pyx":157
+    /* "_curly.pyx":159
  *                 data.data = NULL
  * 
  *         queue_append_last(&ctx_result, data)             # <<<<<<<<<<<<<<
  *         SDL_AtomicIncRef(&dl_ready_to_process)
  * 
  */
     (void)(__pyx_f_6_curly_queue_append_last((&__pyx_v_6_curly_ctx_result), __pyx_v_data));
 
-    /* "_curly.pyx":158
+    /* "_curly.pyx":160
  * 
  *         queue_append_last(&ctx_result, data)
  *         SDL_AtomicIncRef(&dl_ready_to_process)             # <<<<<<<<<<<<<<
  * 
  *     curl_easy_cleanup(curl)
  */
     SDL_AtomicIncRef((&__pyx_v_6_curly_dl_ready_to_process));
     __pyx_L4_continue:;
   }
 
-  /* "_curly.pyx":160
+  /* "_curly.pyx":162
  *         SDL_AtomicIncRef(&dl_ready_to_process)
  * 
  *     curl_easy_cleanup(curl)             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
   (void)(curl_easy_cleanup(__pyx_v_curl));
 
-  /* "_curly.pyx":161
+  /* "_curly.pyx":163
  * 
  *     curl_easy_cleanup(curl)
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "_curly.pyx":80
+  /* "_curly.pyx":81
  * 
  * 
  * cdef int dl_run_job(void *arg) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         dl_queue_data *data
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "_curly.pyx":164
+/* "_curly.pyx":166
  * 
  * 
  * cdef void dl_init(int num_threads) nogil:             # <<<<<<<<<<<<<<
  *     # prepare the queue and background threads
  *     cdef SDL_Thread *thread
  */
 
 static void __pyx_f_6_curly_dl_init(int __pyx_v_num_threads) {
   SDL_Thread *__pyx_v_thread;
   CYTHON_UNUSED int __pyx_v_index;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "_curly.pyx":169
+  /* "_curly.pyx":171
  *     cdef int index
  *     global dl_sem, dl_running
  *     queue_init(&ctx_download)             # <<<<<<<<<<<<<<
  *     queue_init(&ctx_result)
  *     queue_init(&ctx_thread)
  */
   __pyx_f_6_curly_queue_init((&__pyx_v_6_curly_ctx_download));
 
-  /* "_curly.pyx":170
+  /* "_curly.pyx":172
  *     global dl_sem, dl_running
  *     queue_init(&ctx_download)
  *     queue_init(&ctx_result)             # <<<<<<<<<<<<<<
  *     queue_init(&ctx_thread)
  *     SDL_AtomicSet(&dl_done, 0)
  */
   __pyx_f_6_curly_queue_init((&__pyx_v_6_curly_ctx_result));
 
-  /* "_curly.pyx":171
+  /* "_curly.pyx":173
  *     queue_init(&ctx_download)
  *     queue_init(&ctx_result)
  *     queue_init(&ctx_thread)             # <<<<<<<<<<<<<<
  *     SDL_AtomicSet(&dl_done, 0)
  *     dl_sem = SDL_CreateSemaphore(0)
  */
   __pyx_f_6_curly_queue_init((&__pyx_v_6_curly_ctx_thread));
 
-  /* "_curly.pyx":172
+  /* "_curly.pyx":174
  *     queue_init(&ctx_result)
  *     queue_init(&ctx_thread)
  *     SDL_AtomicSet(&dl_done, 0)             # <<<<<<<<<<<<<<
  *     dl_sem = SDL_CreateSemaphore(0)
  * 
  */
   (void)(SDL_AtomicSet((&__pyx_v_6_curly_dl_done), 0));
 
-  /* "_curly.pyx":173
+  /* "_curly.pyx":175
  *     queue_init(&ctx_thread)
  *     SDL_AtomicSet(&dl_done, 0)
  *     dl_sem = SDL_CreateSemaphore(0)             # <<<<<<<<<<<<<<
  * 
  *     curl_global_init(CURL_GLOBAL_ALL)
  */
   __pyx_v_6_curly_dl_sem = SDL_CreateSemaphore(0);
 
-  /* "_curly.pyx":175
+  /* "_curly.pyx":177
  *     dl_sem = SDL_CreateSemaphore(0)
  * 
  *     curl_global_init(CURL_GLOBAL_ALL)             # <<<<<<<<<<<<<<
  * 
  *     for index in range(num_threads):
  */
   (void)(curl_global_init(CURL_GLOBAL_ALL));
 
-  /* "_curly.pyx":177
+  /* "_curly.pyx":179
  *     curl_global_init(CURL_GLOBAL_ALL)
  * 
  *     for index in range(num_threads):             # <<<<<<<<<<<<<<
  *         thread = SDL_CreateThread(dl_run_job, "curl", NULL)
  *         queue_append_last(&ctx_thread, thread)
  */
   __pyx_t_1 = __pyx_v_num_threads;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_index = __pyx_t_3;
 
-    /* "_curly.pyx":178
+    /* "_curly.pyx":180
  * 
  *     for index in range(num_threads):
  *         thread = SDL_CreateThread(dl_run_job, "curl", NULL)             # <<<<<<<<<<<<<<
  *         queue_append_last(&ctx_thread, thread)
  * 
  */
     __pyx_v_thread = SDL_CreateThread(__pyx_f_6_curly_dl_run_job, ((char *)"curl"), NULL);
 
-    /* "_curly.pyx":179
+    /* "_curly.pyx":181
  *     for index in range(num_threads):
  *         thread = SDL_CreateThread(dl_run_job, "curl", NULL)
  *         queue_append_last(&ctx_thread, thread)             # <<<<<<<<<<<<<<
  * 
  *     dl_running = 1
  */
     (void)(__pyx_f_6_curly_queue_append_last((&__pyx_v_6_curly_ctx_thread), __pyx_v_thread));
   }
 
-  /* "_curly.pyx":181
+  /* "_curly.pyx":183
  *         queue_append_last(&ctx_thread, thread)
  * 
  *     dl_running = 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_v_6_curly_dl_running = 1;
 
-  /* "_curly.pyx":164
+  /* "_curly.pyx":166
  * 
  * 
  * cdef void dl_init(int num_threads) nogil:             # <<<<<<<<<<<<<<
  *     # prepare the queue and background threads
  *     cdef SDL_Thread *thread
  */
 
   /* function exit code */
 }
 
-/* "_curly.pyx":184
+/* "_curly.pyx":186
  * 
  * 
  * cdef void dl_ensure_init() nogil:             # <<<<<<<<<<<<<<
  *     # ensure the download threads are ready
  *     if dl_running:
  */
 
 static void __pyx_f_6_curly_dl_ensure_init(void) {
   int __pyx_t_1;
 
-  /* "_curly.pyx":186
+  /* "_curly.pyx":188
  * cdef void dl_ensure_init() nogil:
  *     # ensure the download threads are ready
  *     if dl_running:             # <<<<<<<<<<<<<<
  *         return
  *     dl_init(config_num_threads)
  */
   __pyx_t_1 = (__pyx_v_6_curly_dl_running != 0);
   if (__pyx_t_1) {
 
-    /* "_curly.pyx":187
+    /* "_curly.pyx":189
  *     # ensure the download threads are ready
  *     if dl_running:
  *         return             # <<<<<<<<<<<<<<
  *     dl_init(config_num_threads)
  * 
  */
     goto __pyx_L0;
 
-    /* "_curly.pyx":186
+    /* "_curly.pyx":188
  * cdef void dl_ensure_init() nogil:
  *     # ensure the download threads are ready
  *     if dl_running:             # <<<<<<<<<<<<<<
  *         return
  *     dl_init(config_num_threads)
  */
   }
 
-  /* "_curly.pyx":188
+  /* "_curly.pyx":190
  *     if dl_running:
  *         return
  *     dl_init(config_num_threads)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_f_6_curly_dl_init(__pyx_v_6_curly_config_num_threads);
 
-  /* "_curly.pyx":184
+  /* "_curly.pyx":186
  * 
  * 
  * cdef void dl_ensure_init() nogil:             # <<<<<<<<<<<<<<
  *     # ensure the download threads are ready
  *     if dl_running:
  */
 
   /* function exit code */
   __pyx_L0:;
 }
 
-/* "_curly.pyx":191
+/* "_curly.pyx":193
  * 
  * 
  * def get_info():             # <<<<<<<<<<<<<<
  *     cdef curl_version_info_data *info
  *     dl_ensure_init()
  */
 
@@ -4223,185 +4360,185 @@
   char const *__pyx_t_3;
   char *__pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_info", 0);
 
-  /* "_curly.pyx":193
+  /* "_curly.pyx":195
  * def get_info():
  *     cdef curl_version_info_data *info
  *     dl_ensure_init()             # <<<<<<<<<<<<<<
  *     info = curl_version_info(CURLVERSION_NOW)
  *     ret = {}
  */
   __pyx_f_6_curly_dl_ensure_init();
 
-  /* "_curly.pyx":194
+  /* "_curly.pyx":196
  *     cdef curl_version_info_data *info
  *     dl_ensure_init()
  *     info = curl_version_info(CURLVERSION_NOW)             # <<<<<<<<<<<<<<
  *     ret = {}
  *     if info.version != NULL:
  */
   __pyx_v_info = curl_version_info(CURLVERSION_NOW);
 
-  /* "_curly.pyx":195
+  /* "_curly.pyx":197
  *     dl_ensure_init()
  *     info = curl_version_info(CURLVERSION_NOW)
  *     ret = {}             # <<<<<<<<<<<<<<
  *     if info.version != NULL:
  *         ret["version"] = info.version.decode("utf8")
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ret = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "_curly.pyx":196
+  /* "_curly.pyx":198
  *     info = curl_version_info(CURLVERSION_NOW)
  *     ret = {}
  *     if info.version != NULL:             # <<<<<<<<<<<<<<
  *         ret["version"] = info.version.decode("utf8")
  *     if info.host != NULL:
  */
   __pyx_t_2 = ((__pyx_v_info->version != NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "_curly.pyx":197
+    /* "_curly.pyx":199
  *     ret = {}
  *     if info.version != NULL:
  *         ret["version"] = info.version.decode("utf8")             # <<<<<<<<<<<<<<
  *     if info.host != NULL:
  *         ret["host"] = (<char *>info.host).decode("utf8")
  */
     __pyx_t_3 = __pyx_v_info->version;
-    __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_3, 0, strlen(__pyx_t_3), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_3, 0, strlen(__pyx_t_3), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(PyDict_SetItem(__pyx_v_ret, __pyx_n_s_version, __pyx_t_1) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_ret, __pyx_n_s_version, __pyx_t_1) < 0)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "_curly.pyx":196
+    /* "_curly.pyx":198
  *     info = curl_version_info(CURLVERSION_NOW)
  *     ret = {}
  *     if info.version != NULL:             # <<<<<<<<<<<<<<
  *         ret["version"] = info.version.decode("utf8")
  *     if info.host != NULL:
  */
   }
 
-  /* "_curly.pyx":198
+  /* "_curly.pyx":200
  *     if info.version != NULL:
  *         ret["version"] = info.version.decode("utf8")
  *     if info.host != NULL:             # <<<<<<<<<<<<<<
  *         ret["host"] = (<char *>info.host).decode("utf8")
  *     if info.ssl_version != NULL:
  */
   __pyx_t_2 = ((__pyx_v_info->host != NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "_curly.pyx":199
+    /* "_curly.pyx":201
  *         ret["version"] = info.version.decode("utf8")
  *     if info.host != NULL:
  *         ret["host"] = (<char *>info.host).decode("utf8")             # <<<<<<<<<<<<<<
  *     if info.ssl_version != NULL:
  *         ret["ssl_version"] = (<char *>info.ssl_version).decode("utf8")
  */
     __pyx_t_4 = ((char *)__pyx_v_info->host);
-    __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_4, 0, strlen(__pyx_t_4), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_4, 0, strlen(__pyx_t_4), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(PyDict_SetItem(__pyx_v_ret, __pyx_n_s_host, __pyx_t_1) < 0)) __PYX_ERR(0, 199, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_ret, __pyx_n_s_host, __pyx_t_1) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "_curly.pyx":198
+    /* "_curly.pyx":200
  *     if info.version != NULL:
  *         ret["version"] = info.version.decode("utf8")
  *     if info.host != NULL:             # <<<<<<<<<<<<<<
  *         ret["host"] = (<char *>info.host).decode("utf8")
  *     if info.ssl_version != NULL:
  */
   }
 
-  /* "_curly.pyx":200
+  /* "_curly.pyx":202
  *     if info.host != NULL:
  *         ret["host"] = (<char *>info.host).decode("utf8")
  *     if info.ssl_version != NULL:             # <<<<<<<<<<<<<<
  *         ret["ssl_version"] = (<char *>info.ssl_version).decode("utf8")
  *     if info.libz_version != NULL:
  */
   __pyx_t_2 = ((__pyx_v_info->ssl_version != NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "_curly.pyx":201
+    /* "_curly.pyx":203
  *         ret["host"] = (<char *>info.host).decode("utf8")
  *     if info.ssl_version != NULL:
  *         ret["ssl_version"] = (<char *>info.ssl_version).decode("utf8")             # <<<<<<<<<<<<<<
  *     if info.libz_version != NULL:
  *         ret["libz_version"] = (<char *>info.libz_version).decode("utf8")
  */
     __pyx_t_4 = ((char *)__pyx_v_info->ssl_version);
-    __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_4, 0, strlen(__pyx_t_4), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_4, 0, strlen(__pyx_t_4), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(PyDict_SetItem(__pyx_v_ret, __pyx_n_s_ssl_version, __pyx_t_1) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_ret, __pyx_n_s_ssl_version, __pyx_t_1) < 0)) __PYX_ERR(0, 203, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "_curly.pyx":200
+    /* "_curly.pyx":202
  *     if info.host != NULL:
  *         ret["host"] = (<char *>info.host).decode("utf8")
  *     if info.ssl_version != NULL:             # <<<<<<<<<<<<<<
  *         ret["ssl_version"] = (<char *>info.ssl_version).decode("utf8")
  *     if info.libz_version != NULL:
  */
   }
 
-  /* "_curly.pyx":202
+  /* "_curly.pyx":204
  *     if info.ssl_version != NULL:
  *         ret["ssl_version"] = (<char *>info.ssl_version).decode("utf8")
  *     if info.libz_version != NULL:             # <<<<<<<<<<<<<<
  *         ret["libz_version"] = (<char *>info.libz_version).decode("utf8")
  *     return ret
  */
   __pyx_t_2 = ((__pyx_v_info->libz_version != NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "_curly.pyx":203
+    /* "_curly.pyx":205
  *         ret["ssl_version"] = (<char *>info.ssl_version).decode("utf8")
  *     if info.libz_version != NULL:
  *         ret["libz_version"] = (<char *>info.libz_version).decode("utf8")             # <<<<<<<<<<<<<<
  *     return ret
  * 
  */
     __pyx_t_4 = ((char *)__pyx_v_info->libz_version);
-    __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_4, 0, strlen(__pyx_t_4), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_4, 0, strlen(__pyx_t_4), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(PyDict_SetItem(__pyx_v_ret, __pyx_n_s_libz_version, __pyx_t_1) < 0)) __PYX_ERR(0, 203, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_ret, __pyx_n_s_libz_version, __pyx_t_1) < 0)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "_curly.pyx":202
+    /* "_curly.pyx":204
  *     if info.ssl_version != NULL:
  *         ret["ssl_version"] = (<char *>info.ssl_version).decode("utf8")
  *     if info.libz_version != NULL:             # <<<<<<<<<<<<<<
  *         ret["libz_version"] = (<char *>info.libz_version).decode("utf8")
  *     return ret
  */
   }
 
-  /* "_curly.pyx":204
+  /* "_curly.pyx":206
  *     if info.libz_version != NULL:
  *         ret["libz_version"] = (<char *>info.libz_version).decode("utf8")
  *     return ret             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_ret);
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "_curly.pyx":191
+  /* "_curly.pyx":193
  * 
  * 
  * def get_info():             # <<<<<<<<<<<<<<
  *     cdef curl_version_info_data *info
  *     dl_ensure_init()
  */
 
@@ -4413,15 +4550,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ret);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":207
+/* "_curly.pyx":209
  * 
  * 
  * cdef load_from_surface(SDL_Surface *image):             # <<<<<<<<<<<<<<
  *     # taken from _img_sdl2, just for test.
  *     cdef SDL_Surface *image2 = NULL
  */
 
@@ -4449,407 +4586,407 @@
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("load_from_surface", 0);
 
-  /* "_curly.pyx":209
+  /* "_curly.pyx":211
  * cdef load_from_surface(SDL_Surface *image):
  *     # taken from _img_sdl2, just for test.
  *     cdef SDL_Surface *image2 = NULL             # <<<<<<<<<<<<<<
  *     cdef SDL_Surface *fimage = NULL
  *     cdef SDL_PixelFormat pf
  */
   __pyx_v_image2 = NULL;
 
-  /* "_curly.pyx":210
+  /* "_curly.pyx":212
  *     # taken from _img_sdl2, just for test.
  *     cdef SDL_Surface *image2 = NULL
  *     cdef SDL_Surface *fimage = NULL             # <<<<<<<<<<<<<<
  *     cdef SDL_PixelFormat pf
  *     cdef bytes pixels
  */
   __pyx_v_fimage = NULL;
 
-  /* "_curly.pyx":214
+  /* "_curly.pyx":216
  *     cdef bytes pixels
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         if image == NULL:
  *             return None
  */
   /*try:*/ {
 
-    /* "_curly.pyx":215
+    /* "_curly.pyx":217
  * 
  *     try:
  *         if image == NULL:             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
     __pyx_t_1 = ((__pyx_v_image == NULL) != 0);
     if (__pyx_t_1) {
 
-      /* "_curly.pyx":216
+      /* "_curly.pyx":218
  *     try:
  *         if image == NULL:
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         fmt = ''
  */
       __Pyx_XDECREF(__pyx_r);
       __pyx_r = Py_None; __Pyx_INCREF(Py_None);
       goto __pyx_L3_return;
 
-      /* "_curly.pyx":215
+      /* "_curly.pyx":217
  * 
  *     try:
  *         if image == NULL:             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
     }
 
-    /* "_curly.pyx":218
+    /* "_curly.pyx":220
  *             return None
  * 
  *         fmt = ''             # <<<<<<<<<<<<<<
  *         if image.format.BytesPerPixel == 3:
  *             fmt = 'rgb'
  */
     __Pyx_INCREF(__pyx_kp_s_);
     __pyx_v_fmt = __pyx_kp_s_;
 
-    /* "_curly.pyx":219
+    /* "_curly.pyx":221
  * 
  *         fmt = ''
  *         if image.format.BytesPerPixel == 3:             # <<<<<<<<<<<<<<
  *             fmt = 'rgb'
  *         elif image.format.BytesPerPixel == 4:
  */
     switch (__pyx_v_image->format->BytesPerPixel) {
       case 3:
 
-      /* "_curly.pyx":220
+      /* "_curly.pyx":222
  *         fmt = ''
  *         if image.format.BytesPerPixel == 3:
  *             fmt = 'rgb'             # <<<<<<<<<<<<<<
  *         elif image.format.BytesPerPixel == 4:
  *             fmt = 'rgba'
  */
       __Pyx_INCREF(__pyx_n_s_rgb);
       __Pyx_DECREF_SET(__pyx_v_fmt, __pyx_n_s_rgb);
 
-      /* "_curly.pyx":219
+      /* "_curly.pyx":221
  * 
  *         fmt = ''
  *         if image.format.BytesPerPixel == 3:             # <<<<<<<<<<<<<<
  *             fmt = 'rgb'
  *         elif image.format.BytesPerPixel == 4:
  */
       break;
       case 4:
 
-      /* "_curly.pyx":222
+      /* "_curly.pyx":224
  *             fmt = 'rgb'
  *         elif image.format.BytesPerPixel == 4:
  *             fmt = 'rgba'             # <<<<<<<<<<<<<<
  * 
  *         # FIXME the format might be 3 or 4, but it doesn't mean it's rgb/rgba.
  */
       __Pyx_INCREF(__pyx_n_s_rgba);
       __Pyx_DECREF_SET(__pyx_v_fmt, __pyx_n_s_rgba);
 
-      /* "_curly.pyx":221
+      /* "_curly.pyx":223
  *         if image.format.BytesPerPixel == 3:
  *             fmt = 'rgb'
  *         elif image.format.BytesPerPixel == 4:             # <<<<<<<<<<<<<<
  *             fmt = 'rgba'
  * 
  */
       break;
       default: break;
     }
 
-    /* "_curly.pyx":229
+    /* "_curly.pyx":231
  *         # some opengl card.
  * 
  *         if fmt not in ('rgb', 'rgba'):             # <<<<<<<<<<<<<<
  *             if fmt == 'rgb':
  *                 pf.format = SDL_PIXELFORMAT_BGR888
  */
     __Pyx_INCREF(__pyx_v_fmt);
     __pyx_t_2 = __pyx_v_fmt;
-    __pyx_t_3 = (__Pyx_PyString_Equals(__pyx_t_2, __pyx_n_s_rgb, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 229, __pyx_L4_error)
+    __pyx_t_3 = (__Pyx_PyString_Equals(__pyx_t_2, __pyx_n_s_rgb, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 231, __pyx_L4_error)
     if (__pyx_t_3) {
     } else {
       __pyx_t_1 = __pyx_t_3;
       goto __pyx_L8_bool_binop_done;
     }
-    __pyx_t_3 = (__Pyx_PyString_Equals(__pyx_t_2, __pyx_n_s_rgba, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 229, __pyx_L4_error)
+    __pyx_t_3 = (__Pyx_PyString_Equals(__pyx_t_2, __pyx_n_s_rgba, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 231, __pyx_L4_error)
     __pyx_t_1 = __pyx_t_3;
     __pyx_L8_bool_binop_done:;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_3 = (__pyx_t_1 != 0);
     if (__pyx_t_3) {
 
-      /* "_curly.pyx":230
+      /* "_curly.pyx":232
  * 
  *         if fmt not in ('rgb', 'rgba'):
  *             if fmt == 'rgb':             # <<<<<<<<<<<<<<
  *                 pf.format = SDL_PIXELFORMAT_BGR888
  *                 fmt = 'rgb'
  */
-      __pyx_t_3 = (__Pyx_PyString_Equals(__pyx_v_fmt, __pyx_n_s_rgb, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 230, __pyx_L4_error)
+      __pyx_t_3 = (__Pyx_PyString_Equals(__pyx_v_fmt, __pyx_n_s_rgb, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 232, __pyx_L4_error)
       if (__pyx_t_3) {
 
-        /* "_curly.pyx":231
+        /* "_curly.pyx":233
  *         if fmt not in ('rgb', 'rgba'):
  *             if fmt == 'rgb':
  *                 pf.format = SDL_PIXELFORMAT_BGR888             # <<<<<<<<<<<<<<
  *                 fmt = 'rgb'
  *             else:
  */
         __pyx_v_pf.format = SDL_PIXELFORMAT_BGR888;
 
-        /* "_curly.pyx":232
+        /* "_curly.pyx":234
  *             if fmt == 'rgb':
  *                 pf.format = SDL_PIXELFORMAT_BGR888
  *                 fmt = 'rgb'             # <<<<<<<<<<<<<<
  *             else:
  *                 pf.format = SDL_PIXELFORMAT_ABGR8888
  */
         __Pyx_INCREF(__pyx_n_s_rgb);
         __Pyx_DECREF_SET(__pyx_v_fmt, __pyx_n_s_rgb);
 
-        /* "_curly.pyx":230
+        /* "_curly.pyx":232
  * 
  *         if fmt not in ('rgb', 'rgba'):
  *             if fmt == 'rgb':             # <<<<<<<<<<<<<<
  *                 pf.format = SDL_PIXELFORMAT_BGR888
  *                 fmt = 'rgb'
  */
         goto __pyx_L10;
       }
 
-      /* "_curly.pyx":234
+      /* "_curly.pyx":236
  *                 fmt = 'rgb'
  *             else:
  *                 pf.format = SDL_PIXELFORMAT_ABGR8888             # <<<<<<<<<<<<<<
  *                 fmt = 'rgba'
  * 
  */
       /*else*/ {
         __pyx_v_pf.format = SDL_PIXELFORMAT_ABGR8888;
 
-        /* "_curly.pyx":235
+        /* "_curly.pyx":237
  *             else:
  *                 pf.format = SDL_PIXELFORMAT_ABGR8888
  *                 fmt = 'rgba'             # <<<<<<<<<<<<<<
  * 
  *             image2 = SDL_ConvertSurfaceFormat(image, pf.format, 0)
  */
         __Pyx_INCREF(__pyx_n_s_rgba);
         __Pyx_DECREF_SET(__pyx_v_fmt, __pyx_n_s_rgba);
       }
       __pyx_L10:;
 
-      /* "_curly.pyx":237
+      /* "_curly.pyx":239
  *                 fmt = 'rgba'
  * 
  *             image2 = SDL_ConvertSurfaceFormat(image, pf.format, 0)             # <<<<<<<<<<<<<<
  *             if image2 == NULL:
  *                 return
  */
       __pyx_v_image2 = SDL_ConvertSurfaceFormat(__pyx_v_image, __pyx_v_pf.format, 0);
 
-      /* "_curly.pyx":238
+      /* "_curly.pyx":240
  * 
  *             image2 = SDL_ConvertSurfaceFormat(image, pf.format, 0)
  *             if image2 == NULL:             # <<<<<<<<<<<<<<
  *                 return
  * 
  */
       __pyx_t_3 = ((__pyx_v_image2 == NULL) != 0);
       if (__pyx_t_3) {
 
-        /* "_curly.pyx":239
+        /* "_curly.pyx":241
  *             image2 = SDL_ConvertSurfaceFormat(image, pf.format, 0)
  *             if image2 == NULL:
  *                 return             # <<<<<<<<<<<<<<
  * 
  *             fimage = image2
  */
         __Pyx_XDECREF(__pyx_r);
         __pyx_r = Py_None; __Pyx_INCREF(Py_None);
         goto __pyx_L3_return;
 
-        /* "_curly.pyx":238
+        /* "_curly.pyx":240
  * 
  *             image2 = SDL_ConvertSurfaceFormat(image, pf.format, 0)
  *             if image2 == NULL:             # <<<<<<<<<<<<<<
  *                 return
  * 
  */
       }
 
-      /* "_curly.pyx":241
+      /* "_curly.pyx":243
  *                 return
  * 
  *             fimage = image2             # <<<<<<<<<<<<<<
  *         else:
  *             if (image.format.Rshift > image.format.Bshift):
  */
       __pyx_v_fimage = __pyx_v_image2;
 
-      /* "_curly.pyx":229
+      /* "_curly.pyx":231
  *         # some opengl card.
  * 
  *         if fmt not in ('rgb', 'rgba'):             # <<<<<<<<<<<<<<
  *             if fmt == 'rgb':
  *                 pf.format = SDL_PIXELFORMAT_BGR888
  */
       goto __pyx_L7;
     }
 
-    /* "_curly.pyx":243
+    /* "_curly.pyx":245
  *             fimage = image2
  *         else:
  *             if (image.format.Rshift > image.format.Bshift):             # <<<<<<<<<<<<<<
  *                 memset(&pf, 0, sizeof(pf))
  *                 pf.BitsPerPixel = 32
  */
     /*else*/ {
       __pyx_t_3 = ((__pyx_v_image->format->Rshift > __pyx_v_image->format->Bshift) != 0);
       if (__pyx_t_3) {
 
-        /* "_curly.pyx":244
+        /* "_curly.pyx":246
  *         else:
  *             if (image.format.Rshift > image.format.Bshift):
  *                 memset(&pf, 0, sizeof(pf))             # <<<<<<<<<<<<<<
  *                 pf.BitsPerPixel = 32
  *                 pf.Rmask = 0x000000FF
  */
         (void)(memset((&__pyx_v_pf), 0, (sizeof(__pyx_v_pf))));
 
-        /* "_curly.pyx":245
+        /* "_curly.pyx":247
  *             if (image.format.Rshift > image.format.Bshift):
  *                 memset(&pf, 0, sizeof(pf))
  *                 pf.BitsPerPixel = 32             # <<<<<<<<<<<<<<
  *                 pf.Rmask = 0x000000FF
  *                 pf.Gmask = 0x0000FF00
  */
         __pyx_v_pf.BitsPerPixel = 32;
 
-        /* "_curly.pyx":246
+        /* "_curly.pyx":248
  *                 memset(&pf, 0, sizeof(pf))
  *                 pf.BitsPerPixel = 32
  *                 pf.Rmask = 0x000000FF             # <<<<<<<<<<<<<<
  *                 pf.Gmask = 0x0000FF00
  *                 pf.Bmask = 0x00FF0000
  */
         __pyx_v_pf.Rmask = 0x000000FF;
 
-        /* "_curly.pyx":247
+        /* "_curly.pyx":249
  *                 pf.BitsPerPixel = 32
  *                 pf.Rmask = 0x000000FF
  *                 pf.Gmask = 0x0000FF00             # <<<<<<<<<<<<<<
  *                 pf.Bmask = 0x00FF0000
  *                 pf.Amask = 0xFF000000
  */
         __pyx_v_pf.Gmask = 0x0000FF00;
 
-        /* "_curly.pyx":248
+        /* "_curly.pyx":250
  *                 pf.Rmask = 0x000000FF
  *                 pf.Gmask = 0x0000FF00
  *                 pf.Bmask = 0x00FF0000             # <<<<<<<<<<<<<<
  *                 pf.Amask = 0xFF000000
  *                 image2 = SDL_ConvertSurface(image, &pf, 0)
  */
         __pyx_v_pf.Bmask = 0x00FF0000;
 
-        /* "_curly.pyx":249
+        /* "_curly.pyx":251
  *                 pf.Gmask = 0x0000FF00
  *                 pf.Bmask = 0x00FF0000
  *                 pf.Amask = 0xFF000000             # <<<<<<<<<<<<<<
  *                 image2 = SDL_ConvertSurface(image, &pf, 0)
  *                 fimage = image2
  */
         __pyx_v_pf.Amask = 0xFF000000;
 
-        /* "_curly.pyx":250
+        /* "_curly.pyx":252
  *                 pf.Bmask = 0x00FF0000
  *                 pf.Amask = 0xFF000000
  *                 image2 = SDL_ConvertSurface(image, &pf, 0)             # <<<<<<<<<<<<<<
  *                 fimage = image2
  *             else:
  */
         __pyx_v_image2 = SDL_ConvertSurface(__pyx_v_image, (&__pyx_v_pf), 0);
 
-        /* "_curly.pyx":251
+        /* "_curly.pyx":253
  *                 pf.Amask = 0xFF000000
  *                 image2 = SDL_ConvertSurface(image, &pf, 0)
  *                 fimage = image2             # <<<<<<<<<<<<<<
  *             else:
  *                 fimage = image
  */
         __pyx_v_fimage = __pyx_v_image2;
 
-        /* "_curly.pyx":243
+        /* "_curly.pyx":245
  *             fimage = image2
  *         else:
  *             if (image.format.Rshift > image.format.Bshift):             # <<<<<<<<<<<<<<
  *                 memset(&pf, 0, sizeof(pf))
  *                 pf.BitsPerPixel = 32
  */
         goto __pyx_L12;
       }
 
-      /* "_curly.pyx":253
+      /* "_curly.pyx":255
  *                 fimage = image2
  *             else:
  *                 fimage = image             # <<<<<<<<<<<<<<
  * 
  *         pixels = (<char *>fimage.pixels)[:fimage.pitch * fimage.h]
  */
       /*else*/ {
         __pyx_v_fimage = __pyx_v_image;
       }
       __pyx_L12:;
     }
     __pyx_L7:;
 
-    /* "_curly.pyx":255
+    /* "_curly.pyx":257
  *                 fimage = image
  * 
  *         pixels = (<char *>fimage.pixels)[:fimage.pitch * fimage.h]             # <<<<<<<<<<<<<<
  *         return (fimage.w, fimage.h, fmt, pixels, fimage.pitch)
  * 
  */
-    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(((char *)__pyx_v_fimage->pixels) + 0, (__pyx_v_fimage->pitch * __pyx_v_fimage->h) - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 255, __pyx_L4_error)
+    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(((char *)__pyx_v_fimage->pixels) + 0, (__pyx_v_fimage->pitch * __pyx_v_fimage->h) - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 257, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_pixels = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "_curly.pyx":256
+    /* "_curly.pyx":258
  * 
  *         pixels = (<char *>fimage.pixels)[:fimage.pitch * fimage.h]
  *         return (fimage.w, fimage.h, fmt, pixels, fimage.pitch)             # <<<<<<<<<<<<<<
  * 
  *     finally:
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_fimage->w); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 256, __pyx_L4_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_fimage->w); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 258, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_fimage->h); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 256, __pyx_L4_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_fimage->h); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 258, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_fimage->pitch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 256, __pyx_L4_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_fimage->pitch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 258, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyTuple_New(5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 256, __pyx_L4_error)
+    __pyx_t_6 = PyTuple_New(5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 258, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4);
     __Pyx_INCREF(__pyx_v_fmt);
     __Pyx_GIVEREF(__pyx_v_fmt);
@@ -4863,15 +5000,15 @@
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
     __pyx_r = __pyx_t_6;
     __pyx_t_6 = 0;
     goto __pyx_L3_return;
   }
 
-  /* "_curly.pyx":259
+  /* "_curly.pyx":261
  * 
  *     finally:
  *         if image2:             # <<<<<<<<<<<<<<
  *             SDL_FreeSurface(image2)
  * 
  */
   /*finally:*/ {
@@ -4893,24 +5030,24 @@
       __Pyx_XGOTREF(__pyx_t_14);
       __Pyx_XGOTREF(__pyx_t_15);
       __pyx_t_7 = __pyx_lineno; __pyx_t_8 = __pyx_clineno; __pyx_t_9 = __pyx_filename;
       {
         __pyx_t_3 = (__pyx_v_image2 != 0);
         if (__pyx_t_3) {
 
-          /* "_curly.pyx":260
+          /* "_curly.pyx":262
  *     finally:
  *         if image2:
  *             SDL_FreeSurface(image2)             # <<<<<<<<<<<<<<
  * 
  * 
  */
           SDL_FreeSurface(__pyx_v_image2);
 
-          /* "_curly.pyx":259
+          /* "_curly.pyx":261
  * 
  *     finally:
  *         if image2:             # <<<<<<<<<<<<<<
  *             SDL_FreeSurface(image2)
  * 
  */
         }
@@ -4931,38 +5068,38 @@
     }
     __pyx_L3_return: {
       __pyx_t_15 = __pyx_r;
       __pyx_r = 0;
       __pyx_t_3 = (__pyx_v_image2 != 0);
       if (__pyx_t_3) {
 
-        /* "_curly.pyx":260
+        /* "_curly.pyx":262
  *     finally:
  *         if image2:
  *             SDL_FreeSurface(image2)             # <<<<<<<<<<<<<<
  * 
  * 
  */
         SDL_FreeSurface(__pyx_v_image2);
 
-        /* "_curly.pyx":259
+        /* "_curly.pyx":261
  * 
  *     finally:
  *         if image2:             # <<<<<<<<<<<<<<
  *             SDL_FreeSurface(image2)
  * 
  */
       }
       __pyx_r = __pyx_t_15;
       __pyx_t_15 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "_curly.pyx":207
+  /* "_curly.pyx":209
  * 
  * 
  * cdef load_from_surface(SDL_Surface *image):             # <<<<<<<<<<<<<<
  *     # taken from _img_sdl2, just for test.
  *     cdef SDL_Surface *image2 = NULL
  */
 
@@ -4978,15 +5115,15 @@
   __Pyx_XDECREF(__pyx_v_pixels);
   __Pyx_XDECREF(__pyx_v_fmt);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":265
+/* "_curly.pyx":267
  * class ImageLoaderMemory(ImageLoaderBase):
  *     # Internal loader for data loaded from SDL2
  *     def __init__(self, filename, data, **kwargs):             # <<<<<<<<<<<<<<
  *         w, h, fmt, pixels, rowlength = data
  *         self._data = [ImageData(
  */
 
@@ -5027,40 +5164,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_filename)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(0, 265, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(0, 267, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(0, 265, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(0, 267, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 265, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 267, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_filename = values[1];
     __pyx_v_data = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 265, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 267, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("_curly.ImageLoaderMemory.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6_curly_17ImageLoaderMemory___init__(__pyx_self, __pyx_v_self, __pyx_v_filename, __pyx_v_data, __pyx_v_kwargs);
@@ -5087,28 +5224,28 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *(*__pyx_t_7)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "_curly.pyx":266
+  /* "_curly.pyx":268
  *     # Internal loader for data loaded from SDL2
  *     def __init__(self, filename, data, **kwargs):
  *         w, h, fmt, pixels, rowlength = data             # <<<<<<<<<<<<<<
  *         self._data = [ImageData(
  *             w, h, fmt, pixels, source=filename, rowlength=rowlength)]
  */
   if ((likely(PyTuple_CheckExact(__pyx_v_data))) || (PyList_CheckExact(__pyx_v_data))) {
     PyObject* sequence = __pyx_v_data;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 5)) {
       if (size > 5) __Pyx_RaiseTooManyValuesError(5);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 266, __pyx_L1_error)
+      __PYX_ERR(0, 268, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 2); 
       __pyx_t_4 = PyTuple_GET_ITEM(sequence, 3); 
@@ -5126,144 +5263,147 @@
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_t_5);
     #else
     {
       Py_ssize_t i;
       PyObject** temps[5] = {&__pyx_t_1,&__pyx_t_2,&__pyx_t_3,&__pyx_t_4,&__pyx_t_5};
       for (i=0; i < 5; i++) {
-        PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 266, __pyx_L1_error)
+        PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 268, __pyx_L1_error)
         __Pyx_GOTREF(item);
         *(temps[i]) = item;
       }
     }
     #endif
   } else {
     Py_ssize_t index = -1;
     PyObject** temps[5] = {&__pyx_t_1,&__pyx_t_2,&__pyx_t_3,&__pyx_t_4,&__pyx_t_5};
-    __pyx_t_6 = PyObject_GetIter(__pyx_v_data); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 266, __pyx_L1_error)
+    __pyx_t_6 = PyObject_GetIter(__pyx_v_data); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 268, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = Py_TYPE(__pyx_t_6)->tp_iternext;
     for (index=0; index < 5; index++) {
       PyObject* item = __pyx_t_7(__pyx_t_6); if (unlikely(!item)) goto __pyx_L3_unpacking_failed;
       __Pyx_GOTREF(item);
       *(temps[index]) = item;
     }
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 5) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 5) < 0) __PYX_ERR(0, 268, __pyx_L1_error)
     __pyx_t_7 = NULL;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 266, __pyx_L1_error)
+    __PYX_ERR(0, 268, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_w = __pyx_t_1;
   __pyx_t_1 = 0;
   __pyx_v_h = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_fmt = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_pixels = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_v_rowlength = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "_curly.pyx":267
+  /* "_curly.pyx":269
  *     def __init__(self, filename, data, **kwargs):
  *         w, h, fmt, pixels, rowlength = data
  *         self._data = [ImageData(             # <<<<<<<<<<<<<<
  *             w, h, fmt, pixels, source=filename, rowlength=rowlength)]
  *         super(ImageLoaderMemory, self).__init__(filename, **kwargs)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_ImageData); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_ImageData); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "_curly.pyx":268
+  /* "_curly.pyx":270
  *         w, h, fmt, pixels, rowlength = data
  *         self._data = [ImageData(
  *             w, h, fmt, pixels, source=filename, rowlength=rowlength)]             # <<<<<<<<<<<<<<
  *         super(ImageLoaderMemory, self).__init__(filename, **kwargs)
  * 
  */
-  __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_v_w);
   __Pyx_GIVEREF(__pyx_v_w);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_w);
   __Pyx_INCREF(__pyx_v_h);
   __Pyx_GIVEREF(__pyx_v_h);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_h);
   __Pyx_INCREF(__pyx_v_fmt);
   __Pyx_GIVEREF(__pyx_v_fmt);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_v_fmt);
   __Pyx_INCREF(__pyx_v_pixels);
   __Pyx_GIVEREF(__pyx_v_pixels);
   PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_v_pixels);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_source, __pyx_v_filename) < 0) __PYX_ERR(0, 268, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_rowlength, __pyx_v_rowlength) < 0) __PYX_ERR(0, 268, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_source, __pyx_v_filename) < 0) __PYX_ERR(0, 270, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_rowlength, __pyx_v_rowlength) < 0) __PYX_ERR(0, 270, __pyx_L1_error)
 
-  /* "_curly.pyx":267
+  /* "_curly.pyx":269
  *     def __init__(self, filename, data, **kwargs):
  *         w, h, fmt, pixels, rowlength = data
  *         self._data = [ImageData(             # <<<<<<<<<<<<<<
  *             w, h, fmt, pixels, source=filename, rowlength=rowlength)]
  *         super(ImageLoaderMemory, self).__init__(filename, **kwargs)
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data_2, __pyx_t_3) < 0) __PYX_ERR(0, 267, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data_2, __pyx_t_3) < 0) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "_curly.pyx":269
+  /* "_curly.pyx":271
  *         self._data = [ImageData(
  *             w, h, fmt, pixels, source=filename, rowlength=rowlength)]
  *         super(ImageLoaderMemory, self).__init__(filename, **kwargs)             # <<<<<<<<<<<<<<
  * 
  *     def load(self, kwargs):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ImageLoaderMemory); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ImageLoaderMemory); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
   __Pyx_INCREF(__pyx_v_self);
   __Pyx_GIVEREF(__pyx_v_self);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_self);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_filename);
   __Pyx_GIVEREF(__pyx_v_filename);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_filename);
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_4 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "_curly.pyx":265
+  /* "_curly.pyx":267
  * class ImageLoaderMemory(ImageLoaderBase):
  *     # Internal loader for data loaded from SDL2
  *     def __init__(self, filename, data, **kwargs):             # <<<<<<<<<<<<<<
  *         w, h, fmt, pixels, rowlength = data
  *         self._data = [ImageData(
  */
 
@@ -5286,15 +5426,15 @@
   __Pyx_XDECREF(__pyx_v_pixels);
   __Pyx_XDECREF(__pyx_v_rowlength);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":271
+/* "_curly.pyx":273
  *         super(ImageLoaderMemory, self).__init__(filename, **kwargs)
  * 
  *     def load(self, kwargs):             # <<<<<<<<<<<<<<
  *         return self._data
  * 
  */
 
@@ -5329,32 +5469,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_kwargs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("load", 1, 2, 2, 1); __PYX_ERR(0, 271, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("load", 1, 2, 2, 1); __PYX_ERR(0, 273, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "load") < 0)) __PYX_ERR(0, 271, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "load") < 0)) __PYX_ERR(0, 273, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_kwargs = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("load", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 271, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("load", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 273, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_curly.ImageLoaderMemory.load", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6_curly_17ImageLoaderMemory_2load(__pyx_self, __pyx_v_self, __pyx_v_kwargs);
 
@@ -5368,29 +5508,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("load", 0);
 
-  /* "_curly.pyx":272
+  /* "_curly.pyx":274
  * 
  *     def load(self, kwargs):
  *         return self._data             # <<<<<<<<<<<<<<
  * 
  * #
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_curly.pyx":271
+  /* "_curly.pyx":273
  *         super(ImageLoaderMemory, self).__init__(filename, **kwargs)
  * 
  *     def load(self, kwargs):             # <<<<<<<<<<<<<<
  *         return self._data
  * 
  */
 
@@ -5401,15 +5541,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":302
+/* "_curly.pyx":304
  *         object _http_status_code
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self._data = NULL
  * 
  */
 
@@ -5430,38 +5570,38 @@
 }
 
 static int __pyx_pf_6_curly_11CurlyResult___cinit__(struct __pyx_obj_6_curly_CurlyResult *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "_curly.pyx":303
+  /* "_curly.pyx":305
  * 
  *     def __cinit__(self):
  *         self._data = NULL             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self):
  */
   __pyx_v_self->_data = NULL;
 
-  /* "_curly.pyx":302
+  /* "_curly.pyx":304
  *         object _http_status_code
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self._data = NULL
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":305
+/* "_curly.pyx":307
  *         self._data = NULL
  * 
  *     def __init__(self):             # <<<<<<<<<<<<<<
  *         self._headers = None
  *         self._json = None
  */
 
@@ -5482,81 +5622,81 @@
 }
 
 static int __pyx_pf_6_curly_11CurlyResult_2__init__(struct __pyx_obj_6_curly_CurlyResult *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "_curly.pyx":306
+  /* "_curly.pyx":308
  * 
  *     def __init__(self):
  *         self._headers = None             # <<<<<<<<<<<<<<
  *         self._json = None
  *         self._image = None
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->_headers);
   __Pyx_DECREF(__pyx_v_self->_headers);
   __pyx_v_self->_headers = ((PyObject*)Py_None);
 
-  /* "_curly.pyx":307
+  /* "_curly.pyx":309
  *     def __init__(self):
  *         self._headers = None
  *         self._json = None             # <<<<<<<<<<<<<<
  *         self._image = None
  *         self._reason = None
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->_json);
   __Pyx_DECREF(__pyx_v_self->_json);
   __pyx_v_self->_json = Py_None;
 
-  /* "_curly.pyx":308
+  /* "_curly.pyx":310
  *         self._headers = None
  *         self._json = None
  *         self._image = None             # <<<<<<<<<<<<<<
  *         self._reason = None
  * 
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->_image);
   __Pyx_DECREF(__pyx_v_self->_image);
   __pyx_v_self->_image = Py_None;
 
-  /* "_curly.pyx":309
+  /* "_curly.pyx":311
  *         self._json = None
  *         self._image = None
  *         self._reason = None             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->_reason);
   __Pyx_DECREF(__pyx_v_self->_reason);
   __pyx_v_self->_reason = ((PyObject*)Py_None);
 
-  /* "_curly.pyx":305
+  /* "_curly.pyx":307
  *         self._data = NULL
  * 
  *     def __init__(self):             # <<<<<<<<<<<<<<
  *         self._headers = None
  *         self._json = None
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":311
+/* "_curly.pyx":313
  *         self._reason = None
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         if self._data != NULL:
  *             dl_queue_node_free(&self._data)
  */
 
@@ -5572,77 +5712,77 @@
 }
 
 static void __pyx_pf_6_curly_11CurlyResult_4__dealloc__(struct __pyx_obj_6_curly_CurlyResult *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "_curly.pyx":312
+  /* "_curly.pyx":314
  * 
  *     def __dealloc__(self):
  *         if self._data != NULL:             # <<<<<<<<<<<<<<
  *             dl_queue_node_free(&self._data)
  *             self._data = NULL
  */
   __pyx_t_1 = ((__pyx_v_self->_data != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "_curly.pyx":313
+    /* "_curly.pyx":315
  *     def __dealloc__(self):
  *         if self._data != NULL:
  *             dl_queue_node_free(&self._data)             # <<<<<<<<<<<<<<
  *             self._data = NULL
  *         self._image = None
  */
     __pyx_f_6_curly_dl_queue_node_free((&__pyx_v_self->_data));
 
-    /* "_curly.pyx":314
+    /* "_curly.pyx":316
  *         if self._data != NULL:
  *             dl_queue_node_free(&self._data)
  *             self._data = NULL             # <<<<<<<<<<<<<<
  *         self._image = None
  * 
  */
     __pyx_v_self->_data = NULL;
 
-    /* "_curly.pyx":312
+    /* "_curly.pyx":314
  * 
  *     def __dealloc__(self):
  *         if self._data != NULL:             # <<<<<<<<<<<<<<
  *             dl_queue_node_free(&self._data)
  *             self._data = NULL
  */
   }
 
-  /* "_curly.pyx":315
+  /* "_curly.pyx":317
  *             dl_queue_node_free(&self._data)
  *             self._data = NULL
  *         self._image = None             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->_image);
   __Pyx_DECREF(__pyx_v_self->_image);
   __pyx_v_self->_image = Py_None;
 
-  /* "_curly.pyx":311
+  /* "_curly.pyx":313
  *         self._reason = None
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         if self._data != NULL:
  *             dl_queue_node_free(&self._data)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "_curly.pyx":318
+/* "_curly.pyx":320
  * 
  *     @property
  *     def image(self):             # <<<<<<<<<<<<<<
  *         """Return the CoreImage associated to the url
  *         Only if preload_image was used
  */
 
@@ -5674,131 +5814,131 @@
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "_curly.pyx":322
+  /* "_curly.pyx":324
  *         Only if preload_image was used
  *         """
  *         if self._image is not None:             # <<<<<<<<<<<<<<
  *             return self._image
  * 
  */
   __pyx_t_1 = (__pyx_v_self->_image != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "_curly.pyx":323
+    /* "_curly.pyx":325
  *         """
  *         if self._image is not None:
  *             return self._image             # <<<<<<<<<<<<<<
  * 
  *         if not self._data.preload_image:
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_self->_image);
     __pyx_r = __pyx_v_self->_image;
     goto __pyx_L0;
 
-    /* "_curly.pyx":322
+    /* "_curly.pyx":324
  *         Only if preload_image was used
  *         """
  *         if self._image is not None:             # <<<<<<<<<<<<<<
  *             return self._image
  * 
  */
   }
 
-  /* "_curly.pyx":325
+  /* "_curly.pyx":327
  *             return self._image
  * 
  *         if not self._data.preload_image:             # <<<<<<<<<<<<<<
  *             raise Exception("Preload image not used")
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_self->_data->preload_image != 0)) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "_curly.pyx":326
+    /* "_curly.pyx":328
  * 
  *         if not self._data.preload_image:
  *             raise Exception("Preload image not used")             # <<<<<<<<<<<<<<
  * 
  *         # send back an image
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 326, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 326, __pyx_L1_error)
+    __PYX_ERR(0, 328, __pyx_L1_error)
 
-    /* "_curly.pyx":325
+    /* "_curly.pyx":327
  *             return self._image
  * 
  *         if not self._data.preload_image:             # <<<<<<<<<<<<<<
  *             raise Exception("Preload image not used")
  * 
  */
   }
 
-  /* "_curly.pyx":333
+  /* "_curly.pyx":335
  *         # So using the load_from_surface will disapear somehow to have
  *         # a fully C version that doesn't require python.
  *         if self._data.image == NULL:             # <<<<<<<<<<<<<<
  *             return
  *         image = load_from_surface(self._data.image)
  */
   __pyx_t_2 = ((__pyx_v_self->_data->image == NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "_curly.pyx":334
+    /* "_curly.pyx":336
  *         # a fully C version that doesn't require python.
  *         if self._data.image == NULL:
  *             return             # <<<<<<<<<<<<<<
  *         image = load_from_surface(self._data.image)
  *         loader = ImageLoaderMemory(self._data.url.decode("utf8"), image)
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "_curly.pyx":333
+    /* "_curly.pyx":335
  *         # So using the load_from_surface will disapear somehow to have
  *         # a fully C version that doesn't require python.
  *         if self._data.image == NULL:             # <<<<<<<<<<<<<<
  *             return
  *         image = load_from_surface(self._data.image)
  */
   }
 
-  /* "_curly.pyx":335
+  /* "_curly.pyx":337
  *         if self._data.image == NULL:
  *             return
  *         image = load_from_surface(self._data.image)             # <<<<<<<<<<<<<<
  *         loader = ImageLoaderMemory(self._data.url.decode("utf8"), image)
  *         self._image = CoreImage(loader, nocache=self._data.no_image_cache)
  */
-  __pyx_t_3 = __pyx_f_6_curly_load_from_surface(__pyx_v_self->_data->image); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_6_curly_load_from_surface(__pyx_v_self->_data->image); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_image = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "_curly.pyx":336
+  /* "_curly.pyx":338
  *             return
  *         image = load_from_surface(self._data.image)
  *         loader = ImageLoaderMemory(self._data.url.decode("utf8"), image)             # <<<<<<<<<<<<<<
  *         self._image = CoreImage(loader, nocache=self._data.no_image_cache)
  *         return self._image
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_ImageLoaderMemory); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_ImageLoaderMemory); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = __pyx_v_self->_data->url;
-  __pyx_t_6 = __Pyx_decode_c_string(__pyx_t_5, 0, strlen(__pyx_t_5), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_decode_c_string(__pyx_t_5, 0, strlen(__pyx_t_5), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -5807,94 +5947,94 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_image};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 336, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_image};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 336, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 336, __pyx_L1_error)
+    __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_INCREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_6);
     __Pyx_INCREF(__pyx_v_image);
     __Pyx_GIVEREF(__pyx_v_image);
     PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_image);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 336, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_loader = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "_curly.pyx":337
+  /* "_curly.pyx":339
  *         image = load_from_surface(self._data.image)
  *         loader = ImageLoaderMemory(self._data.url.decode("utf8"), image)
  *         self._image = CoreImage(loader, nocache=self._data.no_image_cache)             # <<<<<<<<<<<<<<
  *         return self._image
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_CoreImage); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_CoreImage); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_v_loader);
   __Pyx_GIVEREF(__pyx_v_loader);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_loader);
-  __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_self->_data->no_image_cache); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_self->_data->no_image_cache); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_nocache, __pyx_t_6) < 0) __PYX_ERR(0, 337, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_nocache, __pyx_t_6) < 0) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_GIVEREF(__pyx_t_6);
   __Pyx_GOTREF(__pyx_v_self->_image);
   __Pyx_DECREF(__pyx_v_self->_image);
   __pyx_v_self->_image = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "_curly.pyx":338
+  /* "_curly.pyx":340
  *         loader = ImageLoaderMemory(self._data.url.decode("utf8"), image)
  *         self._image = CoreImage(loader, nocache=self._data.no_image_cache)
  *         return self._image             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_image);
   __pyx_r = __pyx_v_self->_image;
   goto __pyx_L0;
 
-  /* "_curly.pyx":318
+  /* "_curly.pyx":320
  * 
  *     @property
  *     def image(self):             # <<<<<<<<<<<<<<
  *         """Return the CoreImage associated to the url
  *         Only if preload_image was used
  */
 
@@ -5911,15 +6051,15 @@
   __Pyx_XDECREF(__pyx_v_image);
   __Pyx_XDECREF(__pyx_v_loader);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":342
+/* "_curly.pyx":344
  * 
  *     @property
  *     def url(self):             # <<<<<<<<<<<<<<
  *         """Return the url of the result
  *         """
  */
 
@@ -5942,31 +6082,31 @@
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "_curly.pyx":345
+  /* "_curly.pyx":347
  *         """Return the url of the result
  *         """
  *         return self._data.url.decode("utf8")             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_v_self->_data->url;
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "_curly.pyx":342
+  /* "_curly.pyx":344
  * 
  *     @property
  *     def url(self):             # <<<<<<<<<<<<<<
  *         """Return the url of the result
  *         """
  */
 
@@ -5977,15 +6117,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":348
+/* "_curly.pyx":350
  * 
  *     @property
  *     def error(self):             # <<<<<<<<<<<<<<
  *         """Error message if anything wrong happened
  *         """
  */
 
@@ -6009,50 +6149,50 @@
   char *__pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "_curly.pyx":351
+  /* "_curly.pyx":353
  *         """Error message if anything wrong happened
  *         """
  *         if self._data.image_error != NULL:             # <<<<<<<<<<<<<<
  *             return self._data.image_error.decode("utf8")
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->_data->image_error != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "_curly.pyx":352
+    /* "_curly.pyx":354
  *         """
  *         if self._data.image_error != NULL:
  *             return self._data.image_error.decode("utf8")             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __pyx_v_self->_data->image_error;
-    __pyx_t_3 = __Pyx_decode_c_string(__pyx_t_2, 0, strlen(__pyx_t_2), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 352, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_decode_c_string(__pyx_t_2, 0, strlen(__pyx_t_2), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "_curly.pyx":351
+    /* "_curly.pyx":353
  *         """Error message if anything wrong happened
  *         """
  *         if self._data.image_error != NULL:             # <<<<<<<<<<<<<<
  *             return self._data.image_error.decode("utf8")
  * 
  */
   }
 
-  /* "_curly.pyx":348
+  /* "_curly.pyx":350
  * 
  *     @property
  *     def error(self):             # <<<<<<<<<<<<<<
  *         """Error message if anything wrong happened
  *         """
  */
 
@@ -6065,15 +6205,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":355
+/* "_curly.pyx":357
  * 
  *     @property
  *     def status_code(self):             # <<<<<<<<<<<<<<
  *         """HTTP Status Code
  *         """
  */
 
@@ -6097,53 +6237,53 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "_curly.pyx":358
+  /* "_curly.pyx":360
  *         """HTTP Status Code
  *         """
  *         self._parse_headers()             # <<<<<<<<<<<<<<
  *         return self._http_status_code
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_parse_headers); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_parse_headers); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 360, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 358, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 360, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_curly.pyx":359
+  /* "_curly.pyx":361
  *         """
  *         self._parse_headers()
  *         return self._http_status_code             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_http_status_code);
   __pyx_r = __pyx_v_self->_http_status_code;
   goto __pyx_L0;
 
-  /* "_curly.pyx":355
+  /* "_curly.pyx":357
  * 
  *     @property
  *     def status_code(self):             # <<<<<<<<<<<<<<
  *         """HTTP Status Code
  *         """
  */
 
@@ -6156,15 +6296,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":362
+/* "_curly.pyx":364
  * 
  *     @property
  *     def curl_ret(self):             # <<<<<<<<<<<<<<
  *         """Libcurl status after performing the request.
  *         0 is OK, everything else is an error.
  */
 
@@ -6186,29 +6326,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "_curly.pyx":368
+  /* "_curly.pyx":370
  *         Check https://curl.haxx.se/libcurl/c/libcurl-errors.html
  *         """
  *         return self._data.curl_ret             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_data->curl_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 368, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_data->curl_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_curly.pyx":362
+  /* "_curly.pyx":364
  * 
  *     @property
  *     def curl_ret(self):             # <<<<<<<<<<<<<<
  *         """Libcurl status after performing the request.
  *         0 is OK, everything else is an error.
  */
 
@@ -6219,15 +6359,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":371
+/* "_curly.pyx":373
  * 
  *     @property
  *     def headers(self):             # <<<<<<<<<<<<<<
  *         """HTTP Response headers
  *         """
  */
 
@@ -6251,53 +6391,53 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "_curly.pyx":374
+  /* "_curly.pyx":376
  *         """HTTP Response headers
  *         """
  *         self._parse_headers()             # <<<<<<<<<<<<<<
  *         return self._headers
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_parse_headers); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_parse_headers); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 376, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 376, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_curly.pyx":375
+  /* "_curly.pyx":377
  *         """
  *         self._parse_headers()
  *         return self._headers             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_headers);
   __pyx_r = __pyx_v_self->_headers;
   goto __pyx_L0;
 
-  /* "_curly.pyx":371
+  /* "_curly.pyx":373
  * 
  *     @property
  *     def headers(self):             # <<<<<<<<<<<<<<
  *         """HTTP Response headers
  *         """
  */
 
@@ -6310,15 +6450,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":378
+/* "_curly.pyx":380
  * 
  *     @property
  *     def reason(self):             # <<<<<<<<<<<<<<
  *         """HTTP Reason
  *         """
  */
 
@@ -6342,59 +6482,59 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "_curly.pyx":381
+  /* "_curly.pyx":383
  *         """HTTP Reason
  *         """
  *         self._parse_headers()             # <<<<<<<<<<<<<<
  *         return self._reason.decode("utf8")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_parse_headers); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_parse_headers); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 381, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_curly.pyx":382
+  /* "_curly.pyx":384
  *         """
  *         self._parse_headers()
  *         return self._reason.decode("utf8")             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(__pyx_v_self->_reason == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "decode");
-    __PYX_ERR(0, 382, __pyx_L1_error)
+    __PYX_ERR(0, 384, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_decode_bytes(__pyx_v_self->_reason, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_bytes(__pyx_v_self->_reason, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 384, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_curly.pyx":378
+  /* "_curly.pyx":380
  * 
  *     @property
  *     def reason(self):             # <<<<<<<<<<<<<<
  *         """HTTP Reason
  *         """
  */
 
@@ -6407,15 +6547,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":385
+/* "_curly.pyx":387
  * 
  *     @property
  *     def data(self):             # <<<<<<<<<<<<<<
  *         """HTTP Data from the request
  *         """
  */
 
@@ -6439,58 +6579,58 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "_curly.pyx":389
+  /* "_curly.pyx":391
  *         """
  *         cdef bytes b_data
  *         if self._data.size > 0:             # <<<<<<<<<<<<<<
  *             b_data = self._data.data[:self._data.size]
  *             return b_data
  */
   __pyx_t_1 = ((__pyx_v_self->_data->size > 0) != 0);
   if (__pyx_t_1) {
 
-    /* "_curly.pyx":390
+    /* "_curly.pyx":392
  *         cdef bytes b_data
  *         if self._data.size > 0:
  *             b_data = self._data.data[:self._data.size]             # <<<<<<<<<<<<<<
  *             return b_data
  * 
  */
-    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_self->_data->data + 0, __pyx_v_self->_data->size - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 390, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_self->_data->data + 0, __pyx_v_self->_data->size - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_b_data = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "_curly.pyx":391
+    /* "_curly.pyx":393
  *         if self._data.size > 0:
  *             b_data = self._data.data[:self._data.size]
  *             return b_data             # <<<<<<<<<<<<<<
  * 
  *     def _parse_headers(self):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_b_data);
     __pyx_r = __pyx_v_b_data;
     goto __pyx_L0;
 
-    /* "_curly.pyx":389
+    /* "_curly.pyx":391
  *         """
  *         cdef bytes b_data
  *         if self._data.size > 0:             # <<<<<<<<<<<<<<
  *             b_data = self._data.data[:self._data.size]
  *             return b_data
  */
   }
 
-  /* "_curly.pyx":385
+  /* "_curly.pyx":387
  * 
  *     @property
  *     def data(self):             # <<<<<<<<<<<<<<
  *         """HTTP Data from the request
  *         """
  */
 
@@ -6504,15 +6644,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_b_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":393
+/* "_curly.pyx":395
  *             return b_data
  * 
  *     def _parse_headers(self):             # <<<<<<<<<<<<<<
  *         cdef curl_slist *item
  *         cdef bytes b_data
  */
 
@@ -6546,395 +6686,395 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *(*__pyx_t_8)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_parse_headers", 0);
 
-  /* "_curly.pyx":396
+  /* "_curly.pyx":398
  *         cdef curl_slist *item
  *         cdef bytes b_data
  *         if self._headers is not None:             # <<<<<<<<<<<<<<
  *             return
  *         self._headers = {}
  */
   __pyx_t_1 = (__pyx_v_self->_headers != ((PyObject*)Py_None));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "_curly.pyx":397
+    /* "_curly.pyx":399
  *         cdef bytes b_data
  *         if self._headers is not None:
  *             return             # <<<<<<<<<<<<<<
  *         self._headers = {}
  *         item = self._data.resp_headers
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "_curly.pyx":396
+    /* "_curly.pyx":398
  *         cdef curl_slist *item
  *         cdef bytes b_data
  *         if self._headers is not None:             # <<<<<<<<<<<<<<
  *             return
  *         self._headers = {}
  */
   }
 
-  /* "_curly.pyx":398
+  /* "_curly.pyx":400
  *         if self._headers is not None:
  *             return
  *         self._headers = {}             # <<<<<<<<<<<<<<
  *         item = self._data.resp_headers
  *         while item != NULL:
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 398, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_headers);
   __Pyx_DECREF(__pyx_v_self->_headers);
   __pyx_v_self->_headers = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "_curly.pyx":399
+  /* "_curly.pyx":401
  *             return
  *         self._headers = {}
  *         item = self._data.resp_headers             # <<<<<<<<<<<<<<
  *         while item != NULL:
  *             b_data = item.data[:strlen(item.data)].strip()
  */
   __pyx_t_4 = __pyx_v_self->_data->resp_headers;
   __pyx_v_item = __pyx_t_4;
 
-  /* "_curly.pyx":400
+  /* "_curly.pyx":402
  *         self._headers = {}
  *         item = self._data.resp_headers
  *         while item != NULL:             # <<<<<<<<<<<<<<
  *             b_data = item.data[:strlen(item.data)].strip()
  *             if b_data.startswith(b"HTTP/"):
  */
   while (1) {
     __pyx_t_2 = ((__pyx_v_item != NULL) != 0);
     if (!__pyx_t_2) break;
 
-    /* "_curly.pyx":401
+    /* "_curly.pyx":403
  *         item = self._data.resp_headers
  *         while item != NULL:
  *             b_data = item.data[:strlen(item.data)].strip()             # <<<<<<<<<<<<<<
  *             if b_data.startswith(b"HTTP/"):
  *                 items = b_data.split(b" ", 3)
  */
-    __pyx_t_5 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_item->data + 0, strlen(__pyx_v_item->data) - 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 401, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_item->data + 0, strlen(__pyx_v_item->data) - 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_strip); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 401, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_strip); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 401, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 401, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_b_data, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "_curly.pyx":402
+    /* "_curly.pyx":404
  *         while item != NULL:
  *             b_data = item.data[:strlen(item.data)].strip()
  *             if b_data.startswith(b"HTTP/"):             # <<<<<<<<<<<<<<
  *                 items = b_data.split(b" ", 3)
  *                 self._http_status_code = int(items[1])
  */
     if (unlikely(__pyx_v_b_data == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "startswith");
-      __PYX_ERR(0, 402, __pyx_L1_error)
+      __PYX_ERR(0, 404, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_PyBytes_Tailmatch(__pyx_v_b_data, __pyx_kp_b_HTTP, 0, PY_SSIZE_T_MAX, -1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 402, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_Tailmatch(__pyx_v_b_data, __pyx_kp_b_HTTP, 0, PY_SSIZE_T_MAX, -1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 404, __pyx_L1_error)
     if ((__pyx_t_2 != 0)) {
 
-      /* "_curly.pyx":403
+      /* "_curly.pyx":405
  *             b_data = item.data[:strlen(item.data)].strip()
  *             if b_data.startswith(b"HTTP/"):
  *                 items = b_data.split(b" ", 3)             # <<<<<<<<<<<<<<
  *                 self._http_status_code = int(items[1])
  *                 self._reason = items[-1]
  */
-      __pyx_t_3 = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyBytes_Type_split, __pyx_v_b_data, __pyx_kp_b__3, __pyx_int_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 403, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyBytes_Type_split, __pyx_v_b_data, __pyx_kp_b__3, __pyx_int_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 405, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_XDECREF_SET(__pyx_v_items, __pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "_curly.pyx":404
+      /* "_curly.pyx":406
  *             if b_data.startswith(b"HTTP/"):
  *                 items = b_data.split(b" ", 3)
  *                 self._http_status_code = int(items[1])             # <<<<<<<<<<<<<<
  *                 self._reason = items[-1]
  *             elif b_data:
  */
-      __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_items, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 404, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_items, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_6 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 404, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_GIVEREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_v_self->_http_status_code);
       __Pyx_DECREF(__pyx_v_self->_http_status_code);
       __pyx_v_self->_http_status_code = __pyx_t_6;
       __pyx_t_6 = 0;
 
-      /* "_curly.pyx":405
+      /* "_curly.pyx":407
  *                 items = b_data.split(b" ", 3)
  *                 self._http_status_code = int(items[1])
  *                 self._reason = items[-1]             # <<<<<<<<<<<<<<
  *             elif b_data:
  *                 key, value = b_data.split(b":", 1)
  */
-      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_items, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 405, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_items, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 407, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      if (!(likely(PyBytes_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 405, __pyx_L1_error)
+      if (!(likely(PyBytes_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 407, __pyx_L1_error)
       __Pyx_GIVEREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_v_self->_reason);
       __Pyx_DECREF(__pyx_v_self->_reason);
       __pyx_v_self->_reason = ((PyObject*)__pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "_curly.pyx":402
+      /* "_curly.pyx":404
  *         while item != NULL:
  *             b_data = item.data[:strlen(item.data)].strip()
  *             if b_data.startswith(b"HTTP/"):             # <<<<<<<<<<<<<<
  *                 items = b_data.split(b" ", 3)
  *                 self._http_status_code = int(items[1])
  */
       goto __pyx_L6;
     }
 
-    /* "_curly.pyx":406
+    /* "_curly.pyx":408
  *                 self._http_status_code = int(items[1])
  *                 self._reason = items[-1]
  *             elif b_data:             # <<<<<<<<<<<<<<
  *                 key, value = b_data.split(b":", 1)
  *                 key = key.strip().lower()
  */
     __pyx_t_2 = (__pyx_v_b_data != Py_None)&&(PyBytes_GET_SIZE(__pyx_v_b_data) != 0);
     if (__pyx_t_2) {
 
-      /* "_curly.pyx":407
+      /* "_curly.pyx":409
  *                 self._reason = items[-1]
  *             elif b_data:
  *                 key, value = b_data.split(b":", 1)             # <<<<<<<<<<<<<<
  *                 key = key.strip().lower()
  *                 value = value.strip()
  */
-      __pyx_t_6 = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyBytes_Type_split, __pyx_v_b_data, __pyx_kp_b__4, __pyx_int_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 407, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyBytes_Type_split, __pyx_v_b_data, __pyx_kp_b__4, __pyx_int_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 409, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       if ((likely(PyTuple_CheckExact(__pyx_t_6))) || (PyList_CheckExact(__pyx_t_6))) {
         PyObject* sequence = __pyx_t_6;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 2)) {
           if (size > 2) __Pyx_RaiseTooManyValuesError(2);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 407, __pyx_L1_error)
+          __PYX_ERR(0, 409, __pyx_L1_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
         } else {
           __pyx_t_3 = PyList_GET_ITEM(sequence, 0); 
           __pyx_t_5 = PyList_GET_ITEM(sequence, 1); 
         }
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         #else
-        __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 409, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 407, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 409, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_7 = PyObject_GetIter(__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 407, __pyx_L1_error)
+        __pyx_t_7 = PyObject_GetIter(__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 409, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_t_8 = Py_TYPE(__pyx_t_7)->tp_iternext;
         index = 0; __pyx_t_3 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_3)) goto __pyx_L7_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_3);
         index = 1; __pyx_t_5 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_5)) goto __pyx_L7_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_5);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 2) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 2) < 0) __PYX_ERR(0, 409, __pyx_L1_error)
         __pyx_t_8 = NULL;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         goto __pyx_L8_unpacking_done;
         __pyx_L7_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __pyx_t_8 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 407, __pyx_L1_error)
+        __PYX_ERR(0, 409, __pyx_L1_error)
         __pyx_L8_unpacking_done:;
       }
       __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_3);
       __pyx_t_3 = 0;
       __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "_curly.pyx":408
+      /* "_curly.pyx":410
  *             elif b_data:
  *                 key, value = b_data.split(b":", 1)
  *                 key = key.strip().lower()             # <<<<<<<<<<<<<<
  *                 value = value.strip()
  *                 # XXX is that can potentially break?
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_key, __pyx_n_s_strip); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 408, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_key, __pyx_n_s_strip); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 410, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_7 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 408, __pyx_L1_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 410, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_lower); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 408, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_lower); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 410, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_6 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 408, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 410, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF_SET(__pyx_v_key, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "_curly.pyx":409
+      /* "_curly.pyx":411
  *                 key, value = b_data.split(b":", 1)
  *                 key = key.strip().lower()
  *                 value = value.strip()             # <<<<<<<<<<<<<<
  *                 # XXX is that can potentially break?
  *                 self._headers[key.decode("utf8")] = value.decode("utf8")
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_strip); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 409, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_strip); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_6 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 409, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 411, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "_curly.pyx":411
+      /* "_curly.pyx":413
  *                 value = value.strip()
  *                 # XXX is that can potentially break?
  *                 self._headers[key.decode("utf8")] = value.decode("utf8")             # <<<<<<<<<<<<<<
  *             item = item.next
  * 
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_6 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_s_utf8);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 411, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 413, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (unlikely(__pyx_v_self->_headers == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 411, __pyx_L1_error)
+        __PYX_ERR(0, 413, __pyx_L1_error)
       }
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_key, __pyx_n_s_decode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 411, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_key, __pyx_n_s_decode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 413, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_7 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_s_utf8);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(PyDict_SetItem(__pyx_v_self->_headers, __pyx_t_3, __pyx_t_6) < 0)) __PYX_ERR(0, 411, __pyx_L1_error)
+      if (unlikely(PyDict_SetItem(__pyx_v_self->_headers, __pyx_t_3, __pyx_t_6) < 0)) __PYX_ERR(0, 413, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "_curly.pyx":406
+      /* "_curly.pyx":408
  *                 self._http_status_code = int(items[1])
  *                 self._reason = items[-1]
  *             elif b_data:             # <<<<<<<<<<<<<<
  *                 key, value = b_data.split(b":", 1)
  *                 key = key.strip().lower()
  */
     }
     __pyx_L6:;
 
-    /* "_curly.pyx":412
+    /* "_curly.pyx":414
  *                 # XXX is that can potentially break?
  *                 self._headers[key.decode("utf8")] = value.decode("utf8")
  *             item = item.next             # <<<<<<<<<<<<<<
  * 
  *     def raise_for_status(self):
  */
     __pyx_t_4 = __pyx_v_item->next;
     __pyx_v_item = __pyx_t_4;
   }
 
-  /* "_curly.pyx":393
+  /* "_curly.pyx":395
  *             return b_data
  * 
  *     def _parse_headers(self):             # <<<<<<<<<<<<<<
  *         cdef curl_slist *item
  *         cdef bytes b_data
  */
 
@@ -6954,15 +7094,15 @@
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":414
+/* "_curly.pyx":416
  *             item = item.next
  * 
  *     def raise_for_status(self):             # <<<<<<<<<<<<<<
  *         """If the request failed for any reason, it will raise an
  *         :class:`CurlyError` with the libcurl error code.
  */
 
@@ -6998,259 +7138,259 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("raise_for_status", 0);
 
-  /* "_curly.pyx":423
+  /* "_curly.pyx":425
  * 
  *         cdef const char *c_msg
  *         if self.curl_ret != 0:             # <<<<<<<<<<<<<<
  *             c_msg = curl_easy_strerror(self.curl_ret)
  *             if c_msg == NULL:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_curl_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_curl_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_NeObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_NeObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_3) {
 
-    /* "_curly.pyx":424
+    /* "_curly.pyx":426
  *         cdef const char *c_msg
  *         if self.curl_ret != 0:
  *             c_msg = curl_easy_strerror(self.curl_ret)             # <<<<<<<<<<<<<<
  *             if c_msg == NULL:
  *                 msg = "No error message for {}".format(self.curl_ret)
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_curl_ret); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 424, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_curl_ret); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 426, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 424, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 426, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_c_msg = curl_easy_strerror(__pyx_t_4);
 
-    /* "_curly.pyx":425
+    /* "_curly.pyx":427
  *         if self.curl_ret != 0:
  *             c_msg = curl_easy_strerror(self.curl_ret)
  *             if c_msg == NULL:             # <<<<<<<<<<<<<<
  *                 msg = "No error message for {}".format(self.curl_ret)
  *             else:
  */
     __pyx_t_3 = ((__pyx_v_c_msg == NULL) != 0);
     if (__pyx_t_3) {
 
-      /* "_curly.pyx":426
+      /* "_curly.pyx":428
  *             c_msg = curl_easy_strerror(self.curl_ret)
  *             if c_msg == NULL:
  *                 msg = "No error message for {}".format(self.curl_ret)             # <<<<<<<<<<<<<<
  *             else:
  *                 msg = c_msg.decode("utf8")
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_No_error_message_for, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 426, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_No_error_message_for, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_curl_ret); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 426, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_curl_ret); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 428, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_6 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
         }
       }
       __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 426, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_v_msg = __pyx_t_2;
       __pyx_t_2 = 0;
 
-      /* "_curly.pyx":425
+      /* "_curly.pyx":427
  *         if self.curl_ret != 0:
  *             c_msg = curl_easy_strerror(self.curl_ret)
  *             if c_msg == NULL:             # <<<<<<<<<<<<<<
  *                 msg = "No error message for {}".format(self.curl_ret)
  *             else:
  */
       goto __pyx_L4;
     }
 
-    /* "_curly.pyx":428
+    /* "_curly.pyx":430
  *                 msg = "No error message for {}".format(self.curl_ret)
  *             else:
  *                 msg = c_msg.decode("utf8")             # <<<<<<<<<<<<<<
  *             exc = CurlyError(msg)
  *             exc.code = self.curl_ret
  */
     /*else*/ {
-      __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_c_msg, 0, strlen(__pyx_v_c_msg), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_c_msg, 0, strlen(__pyx_v_c_msg), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_v_msg = __pyx_t_2;
       __pyx_t_2 = 0;
     }
     __pyx_L4:;
 
-    /* "_curly.pyx":429
+    /* "_curly.pyx":431
  *             else:
  *                 msg = c_msg.decode("utf8")
  *             exc = CurlyError(msg)             # <<<<<<<<<<<<<<
  *             exc.code = self.curl_ret
  *             raise exc
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_CurlyError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_CurlyError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 431, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_msg);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 429, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 431, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_exc = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "_curly.pyx":430
+    /* "_curly.pyx":432
  *                 msg = c_msg.decode("utf8")
  *             exc = CurlyError(msg)
  *             exc.code = self.curl_ret             # <<<<<<<<<<<<<<
  *             raise exc
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_curl_ret); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_curl_ret); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 432, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_exc, __pyx_n_s_code, __pyx_t_2) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_exc, __pyx_n_s_code, __pyx_t_2) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "_curly.pyx":431
+    /* "_curly.pyx":433
  *             exc = CurlyError(msg)
  *             exc.code = self.curl_ret
  *             raise exc             # <<<<<<<<<<<<<<
  * 
  *         if self.status_code is None:
  */
     __Pyx_Raise(__pyx_v_exc, 0, 0, 0);
-    __PYX_ERR(0, 431, __pyx_L1_error)
+    __PYX_ERR(0, 433, __pyx_L1_error)
 
-    /* "_curly.pyx":423
+    /* "_curly.pyx":425
  * 
  *         cdef const char *c_msg
  *         if self.curl_ret != 0:             # <<<<<<<<<<<<<<
  *             c_msg = curl_easy_strerror(self.curl_ret)
  *             if c_msg == NULL:
  */
   }
 
-  /* "_curly.pyx":433
+  /* "_curly.pyx":435
  *             raise exc
  * 
  *         if self.status_code is None:             # <<<<<<<<<<<<<<
  *             # no status code, so it's a cached loading
  *             return
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 433, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 435, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = (__pyx_t_2 == Py_None);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_7 = (__pyx_t_3 != 0);
   if (__pyx_t_7) {
 
-    /* "_curly.pyx":435
+    /* "_curly.pyx":437
  *         if self.status_code is None:
  *             # no status code, so it's a cached loading
  *             return             # <<<<<<<<<<<<<<
  * 
  *         reason = None
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "_curly.pyx":433
+    /* "_curly.pyx":435
  *             raise exc
  * 
  *         if self.status_code is None:             # <<<<<<<<<<<<<<
  *             # no status code, so it's a cached loading
  *             return
  */
   }
 
-  /* "_curly.pyx":437
+  /* "_curly.pyx":439
  *             return
  * 
  *         reason = None             # <<<<<<<<<<<<<<
  *         http_error_msg = None
  *         if 400 <= self.status_code < 500:
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_reason = Py_None;
 
-  /* "_curly.pyx":438
+  /* "_curly.pyx":440
  * 
  *         reason = None
  *         http_error_msg = None             # <<<<<<<<<<<<<<
  *         if 400 <= self.status_code < 500:
  *             http_error_msg = u'{} Client Error: {} for url: {}'.format(
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_http_error_msg = Py_None;
 
-  /* "_curly.pyx":439
+  /* "_curly.pyx":441
  *         reason = None
  *         http_error_msg = None
  *         if 400 <= self.status_code < 500:             # <<<<<<<<<<<<<<
  *             http_error_msg = u'{} Client Error: {} for url: {}'.format(
  *                 self.status_code, reason, self.url)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 439, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 441, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_int_400, __pyx_t_2, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 439, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_int_400, __pyx_t_2, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 441, __pyx_L1_error)
   if (__Pyx_PyObject_IsTrue(__pyx_t_1)) {
     __Pyx_DECREF(__pyx_t_1);
-    __pyx_t_1 = PyObject_RichCompare(__pyx_t_2, __pyx_int_500, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 439, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_t_2, __pyx_int_500, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 441, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 439, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 441, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_7) {
 
-    /* "_curly.pyx":440
+    /* "_curly.pyx":442
  *         http_error_msg = None
  *         if 400 <= self.status_code < 500:
  *             http_error_msg = u'{} Client Error: {} for url: {}'.format(             # <<<<<<<<<<<<<<
  *                 self.status_code, reason, self.url)
  *         elif 500 <= self.status_code < 600:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Client_Error_for_url, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 440, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Client_Error_for_url, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 442, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
 
-    /* "_curly.pyx":441
+    /* "_curly.pyx":443
  *         if 400 <= self.status_code < 500:
  *             http_error_msg = u'{} Client Error: {} for url: {}'.format(
  *                 self.status_code, reason, self.url)             # <<<<<<<<<<<<<<
  *         elif 500 <= self.status_code < 600:
  *             http_error_msg = u'{} Server Error: {} for url: {}'.format(
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_status_code); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 441, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_status_code); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 443, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_url); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 441, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_url); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 443, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = NULL;
     __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -7259,103 +7399,103 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_4 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[4] = {__pyx_t_8, __pyx_t_5, __pyx_v_reason, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 440, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 442, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[4] = {__pyx_t_8, __pyx_t_5, __pyx_v_reason, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 440, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 442, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_9 = PyTuple_New(3+__pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 440, __pyx_L1_error)
+      __pyx_t_9 = PyTuple_New(3+__pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 442, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       if (__pyx_t_8) {
         __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_8); __pyx_t_8 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_4, __pyx_t_5);
       __Pyx_INCREF(__pyx_v_reason);
       __Pyx_GIVEREF(__pyx_v_reason);
       PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_4, __pyx_v_reason);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_4, __pyx_t_6);
       __pyx_t_5 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 440, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 442, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_http_error_msg, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "_curly.pyx":439
+    /* "_curly.pyx":441
  *         reason = None
  *         http_error_msg = None
  *         if 400 <= self.status_code < 500:             # <<<<<<<<<<<<<<
  *             http_error_msg = u'{} Client Error: {} for url: {}'.format(
  *                 self.status_code, reason, self.url)
  */
     goto __pyx_L6;
   }
 
-  /* "_curly.pyx":442
+  /* "_curly.pyx":444
  *             http_error_msg = u'{} Client Error: {} for url: {}'.format(
  *                 self.status_code, reason, self.url)
  *         elif 500 <= self.status_code < 600:             # <<<<<<<<<<<<<<
  *             http_error_msg = u'{} Server Error: {} for url: {}'.format(
  *                 self.status_code, reason, self.url)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_status_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 442, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_status_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 444, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_int_500, __pyx_t_1, Py_LE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 442, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_int_500, __pyx_t_1, Py_LE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 444, __pyx_L1_error)
   if (__Pyx_PyObject_IsTrue(__pyx_t_2)) {
     __Pyx_DECREF(__pyx_t_2);
-    __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_int_600, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 442, __pyx_L1_error)
+    __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_int_600, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 444, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 442, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 444, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_7) {
 
-    /* "_curly.pyx":443
+    /* "_curly.pyx":445
  *                 self.status_code, reason, self.url)
  *         elif 500 <= self.status_code < 600:
  *             http_error_msg = u'{} Server Error: {} for url: {}'.format(             # <<<<<<<<<<<<<<
  *                 self.status_code, reason, self.url)
  *         if http_error_msg:
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Server_Error_for_url, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 443, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Server_Error_for_url, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 445, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "_curly.pyx":444
+    /* "_curly.pyx":446
  *         elif 500 <= self.status_code < 600:
  *             http_error_msg = u'{} Server Error: {} for url: {}'.format(
  *                 self.status_code, reason, self.url)             # <<<<<<<<<<<<<<
  *         if http_error_msg:
  *             exc = CurlyHTTPError(http_error_msg)
  */
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_status_code); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 444, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_status_code); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 446, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_url); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 444, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_url); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 446, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_5 = NULL;
     __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -7364,130 +7504,130 @@
         __Pyx_DECREF_SET(__pyx_t_1, function);
         __pyx_t_4 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_1)) {
       PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_t_9, __pyx_v_reason, __pyx_t_6};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 443, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 445, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
       PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_t_9, __pyx_v_reason, __pyx_t_6};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 443, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 445, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_8 = PyTuple_New(3+__pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 443, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(3+__pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 445, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_9);
       PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_4, __pyx_t_9);
       __Pyx_INCREF(__pyx_v_reason);
       __Pyx_GIVEREF(__pyx_v_reason);
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_4, __pyx_v_reason);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_4, __pyx_t_6);
       __pyx_t_9 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 443, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 445, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_http_error_msg, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "_curly.pyx":442
+    /* "_curly.pyx":444
  *             http_error_msg = u'{} Client Error: {} for url: {}'.format(
  *                 self.status_code, reason, self.url)
  *         elif 500 <= self.status_code < 600:             # <<<<<<<<<<<<<<
  *             http_error_msg = u'{} Server Error: {} for url: {}'.format(
  *                 self.status_code, reason, self.url)
  */
   }
   __pyx_L6:;
 
-  /* "_curly.pyx":445
+  /* "_curly.pyx":447
  *             http_error_msg = u'{} Server Error: {} for url: {}'.format(
  *                 self.status_code, reason, self.url)
  *         if http_error_msg:             # <<<<<<<<<<<<<<
  *             exc = CurlyHTTPError(http_error_msg)
  *             exc.response = self
  */
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_v_http_error_msg); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 445, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_v_http_error_msg); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 447, __pyx_L1_error)
   if (unlikely(__pyx_t_7)) {
 
-    /* "_curly.pyx":446
+    /* "_curly.pyx":448
  *                 self.status_code, reason, self.url)
  *         if http_error_msg:
  *             exc = CurlyHTTPError(http_error_msg)             # <<<<<<<<<<<<<<
  *             exc.response = self
  *             raise exc
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_CurlyHTTPError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 446, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_CurlyHTTPError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 448, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_2 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_8, __pyx_v_http_error_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_http_error_msg);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 446, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 448, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_exc = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "_curly.pyx":447
+    /* "_curly.pyx":449
  *         if http_error_msg:
  *             exc = CurlyHTTPError(http_error_msg)
  *             exc.response = self             # <<<<<<<<<<<<<<
  *             raise exc
  * 
  */
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_exc, __pyx_n_s_response, ((PyObject *)__pyx_v_self)) < 0) __PYX_ERR(0, 447, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_exc, __pyx_n_s_response, ((PyObject *)__pyx_v_self)) < 0) __PYX_ERR(0, 449, __pyx_L1_error)
 
-    /* "_curly.pyx":448
+    /* "_curly.pyx":450
  *             exc = CurlyHTTPError(http_error_msg)
  *             exc.response = self
  *             raise exc             # <<<<<<<<<<<<<<
  * 
  *     def json(self):
  */
     __Pyx_Raise(__pyx_v_exc, 0, 0, 0);
-    __PYX_ERR(0, 448, __pyx_L1_error)
+    __PYX_ERR(0, 450, __pyx_L1_error)
 
-    /* "_curly.pyx":445
+    /* "_curly.pyx":447
  *             http_error_msg = u'{} Server Error: {} for url: {}'.format(
  *                 self.status_code, reason, self.url)
  *         if http_error_msg:             # <<<<<<<<<<<<<<
  *             exc = CurlyHTTPError(http_error_msg)
  *             exc.response = self
  */
   }
 
-  /* "_curly.pyx":414
+  /* "_curly.pyx":416
  *             item = item.next
  * 
  *     def raise_for_status(self):             # <<<<<<<<<<<<<<
  *         """If the request failed for any reason, it will raise an
  *         :class:`CurlyError` with the libcurl error code.
  */
 
@@ -7509,15 +7649,15 @@
   __Pyx_XDECREF(__pyx_v_reason);
   __Pyx_XDECREF(__pyx_v_http_error_msg);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":450
+/* "_curly.pyx":452
  *             raise exc
  * 
  *     def json(self):             # <<<<<<<<<<<<<<
  *         """If the content-type is an application/json, then the data will be
  *         interpreted and returned
  */
 
@@ -7545,140 +7685,140 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("json", 0);
 
-  /* "_curly.pyx":454
+  /* "_curly.pyx":456
  *         interpreted and returned
  *         """
  *         if not self.headers.get("content-type", "").startswith("application/json"):             # <<<<<<<<<<<<<<
  *             raise Exception("Not a application/json response")
  *         if self._json is None:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_headers); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_headers); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 456, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 456, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 456, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 456, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_s_application_json) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_application_json);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 454, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 456, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 456, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = ((!__pyx_t_4) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "_curly.pyx":455
+    /* "_curly.pyx":457
  *         """
  *         if not self.headers.get("content-type", "").startswith("application/json"):
  *             raise Exception("Not a application/json response")             # <<<<<<<<<<<<<<
  *         if self._json is None:
  *             self._json = loads(self.data)
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 455, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 455, __pyx_L1_error)
+    __PYX_ERR(0, 457, __pyx_L1_error)
 
-    /* "_curly.pyx":454
+    /* "_curly.pyx":456
  *         interpreted and returned
  *         """
  *         if not self.headers.get("content-type", "").startswith("application/json"):             # <<<<<<<<<<<<<<
  *             raise Exception("Not a application/json response")
  *         if self._json is None:
  */
   }
 
-  /* "_curly.pyx":456
+  /* "_curly.pyx":458
  *         if not self.headers.get("content-type", "").startswith("application/json"):
  *             raise Exception("Not a application/json response")
  *         if self._json is None:             # <<<<<<<<<<<<<<
  *             self._json = loads(self.data)
  *         return self._json
  */
   __pyx_t_5 = (__pyx_v_self->_json == Py_None);
   __pyx_t_4 = (__pyx_t_5 != 0);
   if (__pyx_t_4) {
 
-    /* "_curly.pyx":457
+    /* "_curly.pyx":459
  *             raise Exception("Not a application/json response")
  *         if self._json is None:
  *             self._json = loads(self.data)             # <<<<<<<<<<<<<<
  *         return self._json
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_loads); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 457, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_loads); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 457, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GIVEREF(__pyx_t_1);
     __Pyx_GOTREF(__pyx_v_self->_json);
     __Pyx_DECREF(__pyx_v_self->_json);
     __pyx_v_self->_json = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "_curly.pyx":456
+    /* "_curly.pyx":458
  *         if not self.headers.get("content-type", "").startswith("application/json"):
  *             raise Exception("Not a application/json response")
  *         if self._json is None:             # <<<<<<<<<<<<<<
  *             self._json = loads(self.data)
  *         return self._json
  */
   }
 
-  /* "_curly.pyx":458
+  /* "_curly.pyx":460
  *         if self._json is None:
  *             self._json = loads(self.data)
  *         return self._json             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_json);
   __pyx_r = __pyx_v_self->_json;
   goto __pyx_L0;
 
-  /* "_curly.pyx":450
+  /* "_curly.pyx":452
  *             raise exc
  * 
  *     def json(self):             # <<<<<<<<<<<<<<
  *         """If the content-type is an application/json, then the data will be
  *         interpreted and returned
  */
 
@@ -7692,15 +7832,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":460
+/* "_curly.pyx":462
  *         return self._json
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<CurlyResult url={!r}>".format(self.url)
  * 
  */
 
@@ -7725,47 +7865,47 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "_curly.pyx":461
+  /* "_curly.pyx":463
  * 
  *     def __repr__(self):
  *         return "<CurlyResult url={!r}>".format(self.url)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_CurlyResult_url_r, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_CurlyResult_url_r, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_url); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_url); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_curly.pyx":460
+  /* "_curly.pyx":462
  *         return self._json
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<CurlyResult url={!r}>".format(self.url)
  * 
  */
 
@@ -7892,15 +8032,15 @@
   __Pyx_AddTraceback("_curly.CurlyResult.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":464
+/* "_curly.pyx":466
  * 
  * 
  * def request(url, callback, headers=None,             # <<<<<<<<<<<<<<
  *             method="GET", params=None, data=None, json=None,
  *             auth=None, cache_fn=None, preload_image=False,
  */
 
@@ -7929,37 +8069,37 @@
   __Pyx_RefNannySetupContext("request (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_url,&__pyx_n_s_callback,&__pyx_n_s_headers,&__pyx_n_s_method,&__pyx_n_s_params,&__pyx_n_s_data,&__pyx_n_s_json,&__pyx_n_s_auth,&__pyx_n_s_cache_fn,&__pyx_n_s_preload_image,&__pyx_n_s_priority,&__pyx_n_s_no_image_cache,0};
     PyObject* values[12] = {0,0,0,0,0,0,0,0,0,0,0,0};
     values[2] = ((PyObject *)Py_None);
     values[3] = ((PyObject *)__pyx_n_s_GET);
 
-    /* "_curly.pyx":465
+    /* "_curly.pyx":467
  * 
  * def request(url, callback, headers=None,
  *             method="GET", params=None, data=None, json=None,             # <<<<<<<<<<<<<<
  *             auth=None, cache_fn=None, preload_image=False,
  *             priority=False, no_image_cache=False):
  */
     values[4] = ((PyObject *)Py_None);
     values[5] = ((PyObject *)Py_None);
     values[6] = ((PyObject *)Py_None);
 
-    /* "_curly.pyx":466
+    /* "_curly.pyx":468
  * def request(url, callback, headers=None,
  *             method="GET", params=None, data=None, json=None,
  *             auth=None, cache_fn=None, preload_image=False,             # <<<<<<<<<<<<<<
  *             priority=False, no_image_cache=False):
  *     """Execute an HTTP Request asynchronously.
  */
     values[7] = ((PyObject *)Py_None);
     values[8] = ((PyObject *)Py_None);
     values[9] = ((PyObject *)Py_False);
 
-    /* "_curly.pyx":467
+    /* "_curly.pyx":469
  *             method="GET", params=None, data=None, json=None,
  *             auth=None, cache_fn=None, preload_image=False,
  *             priority=False, no_image_cache=False):             # <<<<<<<<<<<<<<
  *     """Execute an HTTP Request asynchronously.
  *     The result will be dispatched only when :func:`process` is called
  */
     values[10] = ((PyObject *)Py_False);
@@ -8000,15 +8140,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_url)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("request", 0, 2, 12, 1); __PYX_ERR(0, 464, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("request", 0, 2, 12, 1); __PYX_ERR(0, 466, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_headers);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -8064,15 +8204,15 @@
         case 11:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_no_image_cache);
           if (value) { values[11] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "request") < 0)) __PYX_ERR(0, 464, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "request") < 0)) __PYX_ERR(0, 466, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case 12: values[11] = PyTuple_GET_ITEM(__pyx_args, 11);
         CYTHON_FALLTHROUGH;
         case 11: values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
         CYTHON_FALLTHROUGH;
@@ -8109,23 +8249,23 @@
     __pyx_v_cache_fn = values[8];
     __pyx_v_preload_image = values[9];
     __pyx_v_priority = values[10];
     __pyx_v_no_image_cache = values[11];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("request", 0, 2, 12, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 464, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("request", 0, 2, 12, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 466, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_curly.request", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6_curly_2request(__pyx_self, __pyx_v_url, __pyx_v_callback, __pyx_v_headers, __pyx_v_method, __pyx_v_params, __pyx_v_data, __pyx_v_json, __pyx_v_auth, __pyx_v_cache_fn, __pyx_v_preload_image, __pyx_v_priority, __pyx_v_no_image_cache);
 
-  /* "_curly.pyx":464
+  /* "_curly.pyx":466
  * 
  * 
  * def request(url, callback, headers=None,             # <<<<<<<<<<<<<<
  *             method="GET", params=None, data=None, json=None,
  *             auth=None, cache_fn=None, preload_image=False,
  */
 
@@ -8169,294 +8309,294 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("request", 0);
   __Pyx_INCREF(__pyx_v_url);
   __Pyx_INCREF(__pyx_v_data);
 
-  /* "_curly.pyx":518
+  /* "_curly.pyx":520
  *         char *c_header
  * 
  *     if data and json:             # <<<<<<<<<<<<<<
  *         raise Exception("Cannot have data and json parameters at the same time")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_data); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 518, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_data); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 520, __pyx_L1_error)
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_json); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 518, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_json); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 520, __pyx_L1_error)
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "_curly.pyx":519
+    /* "_curly.pyx":521
  * 
  *     if data and json:
  *         raise Exception("Cannot have data and json parameters at the same time")             # <<<<<<<<<<<<<<
  * 
  *     # allocate qdata
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 519, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 521, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 519, __pyx_L1_error)
+    __PYX_ERR(0, 521, __pyx_L1_error)
 
-    /* "_curly.pyx":518
+    /* "_curly.pyx":520
  *         char *c_header
  * 
  *     if data and json:             # <<<<<<<<<<<<<<
  *         raise Exception("Cannot have data and json parameters at the same time")
  * 
  */
   }
 
-  /* "_curly.pyx":522
+  /* "_curly.pyx":524
  * 
  *     # allocate qdata
  *     qdata = <dl_queue_data *>calloc(1, sizeof(dl_queue_data))             # <<<<<<<<<<<<<<
  *     qdata.preload_image = int(preload_image)
  *     qdata.no_image_cache = int(no_image_cache)
  */
   __pyx_v_qdata = ((__pyx_t_6_curly_dl_queue_data *)calloc(1, (sizeof(__pyx_t_6_curly_dl_queue_data))));
 
-  /* "_curly.pyx":523
+  /* "_curly.pyx":525
  *     # allocate qdata
  *     qdata = <dl_queue_data *>calloc(1, sizeof(dl_queue_data))
  *     qdata.preload_image = int(preload_image)             # <<<<<<<<<<<<<<
  *     qdata.no_image_cache = int(no_image_cache)
  * 
  */
-  __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_v_preload_image); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 523, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_v_preload_image); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 525, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 523, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 525, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_qdata->preload_image = __pyx_t_4;
 
-  /* "_curly.pyx":524
+  /* "_curly.pyx":526
  *     qdata = <dl_queue_data *>calloc(1, sizeof(dl_queue_data))
  *     qdata.preload_image = int(preload_image)
  *     qdata.no_image_cache = int(no_image_cache)             # <<<<<<<<<<<<<<
  * 
  *     # url + params
  */
-  __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_v_no_image_cache); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 524, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_v_no_image_cache); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 526, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 524, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 526, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_qdata->no_image_cache = __pyx_t_4;
 
-  /* "_curly.pyx":527
+  /* "_curly.pyx":529
  * 
  *     # url + params
  *     if params:             # <<<<<<<<<<<<<<
  *         url_suffix = []
  *         for key, value in params.items():
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_params); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 527, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_params); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 529, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "_curly.pyx":528
+    /* "_curly.pyx":530
  *     # url + params
  *     if params:
  *         url_suffix = []             # <<<<<<<<<<<<<<
  *         for key, value in params.items():
  *             value = "{}".format(value)
  */
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 528, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 530, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_url_suffix = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "_curly.pyx":529
+    /* "_curly.pyx":531
  *     if params:
  *         url_suffix = []
  *         for key, value in params.items():             # <<<<<<<<<<<<<<
  *             value = "{}".format(value)
  *             url_suffix.append("{}={}".format(quote(key), quote(value)))
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_params, __pyx_n_s_items); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 529, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_params, __pyx_n_s_items); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 531, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 529, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 531, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
       __pyx_t_5 = __pyx_t_3; __Pyx_INCREF(__pyx_t_5); __pyx_t_7 = 0;
       __pyx_t_8 = NULL;
     } else {
-      __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 529, __pyx_L1_error)
+      __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 531, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_8 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 529, __pyx_L1_error)
+      __pyx_t_8 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 531, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     for (;;) {
       if (likely(!__pyx_t_8)) {
         if (likely(PyList_CheckExact(__pyx_t_5))) {
           if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_5)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 529, __pyx_L1_error)
+          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 531, __pyx_L1_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 529, __pyx_L1_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 531, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         } else {
           if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 529, __pyx_L1_error)
+          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 531, __pyx_L1_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 529, __pyx_L1_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 531, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         }
       } else {
         __pyx_t_3 = __pyx_t_8(__pyx_t_5);
         if (unlikely(!__pyx_t_3)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 529, __pyx_L1_error)
+            else __PYX_ERR(0, 531, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_3);
       }
       if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
         PyObject* sequence = __pyx_t_3;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 2)) {
           if (size > 2) __Pyx_RaiseTooManyValuesError(2);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 529, __pyx_L1_error)
+          __PYX_ERR(0, 531, __pyx_L1_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_9 = PyTuple_GET_ITEM(sequence, 1); 
         } else {
           __pyx_t_6 = PyList_GET_ITEM(sequence, 0); 
           __pyx_t_9 = PyList_GET_ITEM(sequence, 1); 
         }
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_9);
         #else
-        __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 529, __pyx_L1_error)
+        __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 531, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_9 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 529, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 531, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_10 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 529, __pyx_L1_error)
+        __pyx_t_10 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 531, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_t_11 = Py_TYPE(__pyx_t_10)->tp_iternext;
         index = 0; __pyx_t_6 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_6)) goto __pyx_L9_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_6);
         index = 1; __pyx_t_9 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_9)) goto __pyx_L9_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_9);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_10), 2) < 0) __PYX_ERR(0, 529, __pyx_L1_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_10), 2) < 0) __PYX_ERR(0, 531, __pyx_L1_error)
         __pyx_t_11 = NULL;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         goto __pyx_L10_unpacking_done;
         __pyx_L9_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         __pyx_t_11 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 529, __pyx_L1_error)
+        __PYX_ERR(0, 531, __pyx_L1_error)
         __pyx_L10_unpacking_done:;
       }
       __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_6);
       __pyx_t_6 = 0;
       __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_9);
       __pyx_t_9 = 0;
 
-      /* "_curly.pyx":530
+      /* "_curly.pyx":532
  *         url_suffix = []
  *         for key, value in params.items():
  *             value = "{}".format(value)             # <<<<<<<<<<<<<<
  *             url_suffix.append("{}={}".format(quote(key), quote(value)))
  *         if "?" in url:
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__10, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 530, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__10, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 532, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_6 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
         }
       }
       __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_6, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_value);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 530, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 532, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "_curly.pyx":531
+      /* "_curly.pyx":533
  *         for key, value in params.items():
  *             value = "{}".format(value)
  *             url_suffix.append("{}={}".format(quote(key), quote(value)))             # <<<<<<<<<<<<<<
  *         if "?" in url:
  *             url += "&" + "&".join(url_suffix)
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__11, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 531, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__11, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 533, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_quote); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 531, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_quote); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 533, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_12 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
         __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_10);
         if (likely(__pyx_t_12)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
           __Pyx_INCREF(__pyx_t_12);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_10, function);
         }
       }
       __pyx_t_6 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_12, __pyx_v_key) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_v_key);
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 531, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 533, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_quote); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 531, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_quote); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 533, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       __pyx_t_13 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
         __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_12);
         if (likely(__pyx_t_13)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
           __Pyx_INCREF(__pyx_t_13);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_12, function);
         }
       }
       __pyx_t_10 = (__pyx_t_13) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_13, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_v_value);
       __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-      if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 531, __pyx_L1_error)
+      if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 533, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __pyx_t_12 = NULL;
       __pyx_t_4 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_12)) {
@@ -8466,519 +8606,519 @@
           __Pyx_DECREF_SET(__pyx_t_9, function);
           __pyx_t_4 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_9)) {
         PyObject *__pyx_temp[3] = {__pyx_t_12, __pyx_t_6, __pyx_t_10};
-        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 531, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 533, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
         PyObject *__pyx_temp[3] = {__pyx_t_12, __pyx_t_6, __pyx_t_10};
-        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 531, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 533, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       } else
       #endif
       {
-        __pyx_t_13 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 531, __pyx_L1_error)
+        __pyx_t_13 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 533, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_13);
         if (__pyx_t_12) {
           __Pyx_GIVEREF(__pyx_t_12); PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_12); __pyx_t_12 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_13, 0+__pyx_t_4, __pyx_t_6);
         __Pyx_GIVEREF(__pyx_t_10);
         PyTuple_SET_ITEM(__pyx_t_13, 1+__pyx_t_4, __pyx_t_10);
         __pyx_t_6 = 0;
         __pyx_t_10 = 0;
-        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 531, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 533, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       }
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __pyx_t_14 = __Pyx_PyList_Append(__pyx_v_url_suffix, __pyx_t_3); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 531, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyList_Append(__pyx_v_url_suffix, __pyx_t_3); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 533, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "_curly.pyx":529
+      /* "_curly.pyx":531
  *     if params:
  *         url_suffix = []
  *         for key, value in params.items():             # <<<<<<<<<<<<<<
  *             value = "{}".format(value)
  *             url_suffix.append("{}={}".format(quote(key), quote(value)))
  */
     }
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "_curly.pyx":532
+    /* "_curly.pyx":534
  *             value = "{}".format(value)
  *             url_suffix.append("{}={}".format(quote(key), quote(value)))
  *         if "?" in url:             # <<<<<<<<<<<<<<
  *             url += "&" + "&".join(url_suffix)
  *         else:
  */
-    __pyx_t_1 = (__Pyx_PySequence_ContainsTF(__pyx_kp_s__12, __pyx_v_url, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 532, __pyx_L1_error)
+    __pyx_t_1 = (__Pyx_PySequence_ContainsTF(__pyx_kp_s__12, __pyx_v_url, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 534, __pyx_L1_error)
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (__pyx_t_2) {
 
-      /* "_curly.pyx":533
+      /* "_curly.pyx":535
  *             url_suffix.append("{}={}".format(quote(key), quote(value)))
  *         if "?" in url:
  *             url += "&" + "&".join(url_suffix)             # <<<<<<<<<<<<<<
  *         else:
  *             url += "?" + "&".join(url_suffix)
  */
-      __pyx_t_5 = __Pyx_PyString_Join(__pyx_kp_s__13, __pyx_v_url_suffix); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 533, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyString_Join(__pyx_kp_s__13, __pyx_v_url_suffix); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 535, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_3 = PyNumber_Add(__pyx_kp_s__13, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 533, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_kp_s__13, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_v_url, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 533, __pyx_L1_error)
+      __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_v_url, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 535, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF_SET(__pyx_v_url, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "_curly.pyx":532
+      /* "_curly.pyx":534
  *             value = "{}".format(value)
  *             url_suffix.append("{}={}".format(quote(key), quote(value)))
  *         if "?" in url:             # <<<<<<<<<<<<<<
  *             url += "&" + "&".join(url_suffix)
  *         else:
  */
       goto __pyx_L11;
     }
 
-    /* "_curly.pyx":535
+    /* "_curly.pyx":537
  *             url += "&" + "&".join(url_suffix)
  *         else:
  *             url += "?" + "&".join(url_suffix)             # <<<<<<<<<<<<<<
  * 
  *     b_string = url.encode("utf8")
  */
     /*else*/ {
-      __pyx_t_5 = __Pyx_PyString_Join(__pyx_kp_s__13, __pyx_v_url_suffix); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 535, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyString_Join(__pyx_kp_s__13, __pyx_v_url_suffix); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 537, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_3 = PyNumber_Add(__pyx_kp_s__12, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_kp_s__12, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 537, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_v_url, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 535, __pyx_L1_error)
+      __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_v_url, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 537, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF_SET(__pyx_v_url, __pyx_t_5);
       __pyx_t_5 = 0;
     }
     __pyx_L11:;
 
-    /* "_curly.pyx":527
+    /* "_curly.pyx":529
  * 
  *     # url + params
  *     if params:             # <<<<<<<<<<<<<<
  *         url_suffix = []
  *         for key, value in params.items():
  */
   }
 
-  /* "_curly.pyx":537
+  /* "_curly.pyx":539
  *             url += "?" + "&".join(url_suffix)
  * 
  *     b_string = url.encode("utf8")             # <<<<<<<<<<<<<<
  *     qdata.url = strdup(b_string)
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_url, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 537, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_url, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 539, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_9, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_s_utf8);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 537, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 539, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 537, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 539, __pyx_L1_error)
   __pyx_v_b_string = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "_curly.pyx":538
+  /* "_curly.pyx":540
  * 
  *     b_string = url.encode("utf8")
  *     qdata.url = strdup(b_string)             # <<<<<<<<<<<<<<
  * 
  *     # method
  */
   if (unlikely(__pyx_v_b_string == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 538, __pyx_L1_error)
+    __PYX_ERR(0, 540, __pyx_L1_error)
   }
-  __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 538, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 540, __pyx_L1_error)
   __pyx_v_qdata->url = strdup(__pyx_t_15);
 
-  /* "_curly.pyx":541
+  /* "_curly.pyx":543
  * 
  *     # method
  *     b_string = method.encode("utf8")             # <<<<<<<<<<<<<<
  *     qdata.method = strdup(b_string)
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_method, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_method, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_9, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_s_utf8);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 541, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 541, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_b_string, ((PyObject*)__pyx_t_5));
   __pyx_t_5 = 0;
 
-  /* "_curly.pyx":542
+  /* "_curly.pyx":544
  *     # method
  *     b_string = method.encode("utf8")
  *     qdata.method = strdup(b_string)             # <<<<<<<<<<<<<<
  * 
  *     # postdata
  */
   if (unlikely(__pyx_v_b_string == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 542, __pyx_L1_error)
+    __PYX_ERR(0, 544, __pyx_L1_error)
   }
-  __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 542, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 544, __pyx_L1_error)
   __pyx_v_qdata->method = strdup(__pyx_t_15);
 
-  /* "_curly.pyx":545
+  /* "_curly.pyx":547
  * 
  *     # postdata
  *     if json is not None:             # <<<<<<<<<<<<<<
  *         data = dumps(json)
  *         b_string = data.encode("utf8")
  */
   __pyx_t_2 = (__pyx_v_json != Py_None);
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "_curly.pyx":546
+    /* "_curly.pyx":548
  *     # postdata
  *     if json is not None:
  *         data = dumps(json)             # <<<<<<<<<<<<<<
  *         b_string = data.encode("utf8")
  *         qdata.postdata = strdup(b_string)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_dumps); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 546, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_dumps); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 548, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_9 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_9, __pyx_v_json) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_json);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 546, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 548, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "_curly.pyx":547
+    /* "_curly.pyx":549
  *     if json is not None:
  *         data = dumps(json)
  *         b_string = data.encode("utf8")             # <<<<<<<<<<<<<<
  *         qdata.postdata = strdup(b_string)
  *         headers["Content-Type"] = "application/json"
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 547, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 549, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_9 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_9, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_s_utf8);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 547, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 549, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 547, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 549, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_b_string, ((PyObject*)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "_curly.pyx":548
+    /* "_curly.pyx":550
  *         data = dumps(json)
  *         b_string = data.encode("utf8")
  *         qdata.postdata = strdup(b_string)             # <<<<<<<<<<<<<<
  *         headers["Content-Type"] = "application/json"
  *     elif isinstance(data, dict):
  */
     if (unlikely(__pyx_v_b_string == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-      __PYX_ERR(0, 548, __pyx_L1_error)
+      __PYX_ERR(0, 550, __pyx_L1_error)
     }
-    __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 548, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 550, __pyx_L1_error)
     __pyx_v_qdata->postdata = strdup(__pyx_t_15);
 
-    /* "_curly.pyx":549
+    /* "_curly.pyx":551
  *         b_string = data.encode("utf8")
  *         qdata.postdata = strdup(b_string)
  *         headers["Content-Type"] = "application/json"             # <<<<<<<<<<<<<<
  *     elif isinstance(data, dict):
  *         # XXX support multipart form-data, using curl_mime
  */
-    if (unlikely(PyObject_SetItem(__pyx_v_headers, __pyx_kp_s_Content_Type, __pyx_kp_s_application_json) < 0)) __PYX_ERR(0, 549, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_headers, __pyx_kp_s_Content_Type, __pyx_kp_s_application_json) < 0)) __PYX_ERR(0, 551, __pyx_L1_error)
 
-    /* "_curly.pyx":545
+    /* "_curly.pyx":547
  * 
  *     # postdata
  *     if json is not None:             # <<<<<<<<<<<<<<
  *         data = dumps(json)
  *         b_string = data.encode("utf8")
  */
     goto __pyx_L12;
   }
 
-  /* "_curly.pyx":550
+  /* "_curly.pyx":552
  *         qdata.postdata = strdup(b_string)
  *         headers["Content-Type"] = "application/json"
  *     elif isinstance(data, dict):             # <<<<<<<<<<<<<<
  *         # XXX support multipart form-data, using curl_mime
  *         postdata = []
  */
   __pyx_t_1 = PyDict_Check(__pyx_v_data); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "_curly.pyx":552
+    /* "_curly.pyx":554
  *     elif isinstance(data, dict):
  *         # XXX support multipart form-data, using curl_mime
  *         postdata = []             # <<<<<<<<<<<<<<
  *         for key, value in data.items():
  *             value = "{}".format(value)
  */
-    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 552, __pyx_L1_error)
+    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 554, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_v_postdata = __pyx_t_5;
     __pyx_t_5 = 0;
 
-    /* "_curly.pyx":553
+    /* "_curly.pyx":555
  *         # XXX support multipart form-data, using curl_mime
  *         postdata = []
  *         for key, value in data.items():             # <<<<<<<<<<<<<<
  *             value = "{}".format(value)
  *             postdata.append("{}={}".format(quote(key), quote(value)))
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_items); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 553, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_items); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 555, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_9 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_9) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 553, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 555, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (likely(PyList_CheckExact(__pyx_t_5)) || PyTuple_CheckExact(__pyx_t_5)) {
       __pyx_t_3 = __pyx_t_5; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
       __pyx_t_8 = NULL;
     } else {
-      __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 553, __pyx_L1_error)
+      __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 555, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 553, __pyx_L1_error)
+      __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 555, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     for (;;) {
       if (likely(!__pyx_t_8)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 553, __pyx_L1_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 555, __pyx_L1_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 553, __pyx_L1_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 555, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 553, __pyx_L1_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 555, __pyx_L1_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 553, __pyx_L1_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 555, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_8(__pyx_t_3);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 553, __pyx_L1_error)
+            else __PYX_ERR(0, 555, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       if ((likely(PyTuple_CheckExact(__pyx_t_5))) || (PyList_CheckExact(__pyx_t_5))) {
         PyObject* sequence = __pyx_t_5;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 2)) {
           if (size > 2) __Pyx_RaiseTooManyValuesError(2);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 553, __pyx_L1_error)
+          __PYX_ERR(0, 555, __pyx_L1_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_9 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_13 = PyTuple_GET_ITEM(sequence, 1); 
         } else {
           __pyx_t_9 = PyList_GET_ITEM(sequence, 0); 
           __pyx_t_13 = PyList_GET_ITEM(sequence, 1); 
         }
         __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(__pyx_t_13);
         #else
-        __pyx_t_9 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 553, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 555, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
-        __pyx_t_13 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 553, __pyx_L1_error)
+        __pyx_t_13 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 555, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_13);
         #endif
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_10 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 553, __pyx_L1_error)
+        __pyx_t_10 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 555, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __pyx_t_11 = Py_TYPE(__pyx_t_10)->tp_iternext;
         index = 0; __pyx_t_9 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_9)) goto __pyx_L15_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_9);
         index = 1; __pyx_t_13 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_13)) goto __pyx_L15_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_13);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_10), 2) < 0) __PYX_ERR(0, 553, __pyx_L1_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_10), 2) < 0) __PYX_ERR(0, 555, __pyx_L1_error)
         __pyx_t_11 = NULL;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         goto __pyx_L16_unpacking_done;
         __pyx_L15_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         __pyx_t_11 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 553, __pyx_L1_error)
+        __PYX_ERR(0, 555, __pyx_L1_error)
         __pyx_L16_unpacking_done:;
       }
       __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_9);
       __pyx_t_9 = 0;
       __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_13);
       __pyx_t_13 = 0;
 
-      /* "_curly.pyx":554
+      /* "_curly.pyx":556
  *         postdata = []
  *         for key, value in data.items():
  *             value = "{}".format(value)             # <<<<<<<<<<<<<<
  *             postdata.append("{}={}".format(quote(key), quote(value)))
  *         postdata = "&".join(postdata)
  */
-      __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__10, __pyx_n_s_format); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 554, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__10, __pyx_n_s_format); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 556, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __pyx_t_9 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_13);
         if (likely(__pyx_t_9)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
           __Pyx_INCREF(__pyx_t_9);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_13, function);
         }
       }
       __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_9, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_v_value);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 554, __pyx_L1_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 556, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "_curly.pyx":555
+      /* "_curly.pyx":557
  *         for key, value in data.items():
  *             value = "{}".format(value)
  *             postdata.append("{}={}".format(quote(key), quote(value)))             # <<<<<<<<<<<<<<
  *         postdata = "&".join(postdata)
  *         b_string = postdata.encode("utf8")
  */
-      __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__11, __pyx_n_s_format); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 555, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__11, __pyx_n_s_format); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 557, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
-      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_quote); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 555, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_quote); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 557, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_6 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_10);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_10, function);
         }
       }
       __pyx_t_9 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_6, __pyx_v_key) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_v_key);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 555, __pyx_L1_error)
+      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 557, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_quote); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 555, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_quote); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 557, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_12 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_12)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
           __Pyx_INCREF(__pyx_t_12);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
         }
       }
       __pyx_t_10 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_12, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_value);
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-      if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 555, __pyx_L1_error)
+      if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 557, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = NULL;
       __pyx_t_4 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_13);
         if (likely(__pyx_t_6)) {
@@ -8988,424 +9128,424 @@
           __Pyx_DECREF_SET(__pyx_t_13, function);
           __pyx_t_4 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_13)) {
         PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_9, __pyx_t_10};
-        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_13, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 555, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_13, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 557, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_13)) {
         PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_9, __pyx_t_10};
-        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_13, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 555, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_13, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 557, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       } else
       #endif
       {
-        __pyx_t_12 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 555, __pyx_L1_error)
+        __pyx_t_12 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 557, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         if (__pyx_t_6) {
           __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_6); __pyx_t_6 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_9);
         PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_4, __pyx_t_9);
         __Pyx_GIVEREF(__pyx_t_10);
         PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_4, __pyx_t_10);
         __pyx_t_9 = 0;
         __pyx_t_10 = 0;
-        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_13, __pyx_t_12, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 555, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_13, __pyx_t_12, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 557, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       }
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-      __pyx_t_14 = __Pyx_PyObject_Append(__pyx_v_postdata, __pyx_t_5); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 555, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyObject_Append(__pyx_v_postdata, __pyx_t_5); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 557, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "_curly.pyx":553
+      /* "_curly.pyx":555
  *         # XXX support multipart form-data, using curl_mime
  *         postdata = []
  *         for key, value in data.items():             # <<<<<<<<<<<<<<
  *             value = "{}".format(value)
  *             postdata.append("{}={}".format(quote(key), quote(value)))
  */
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "_curly.pyx":556
+    /* "_curly.pyx":558
  *             value = "{}".format(value)
  *             postdata.append("{}={}".format(quote(key), quote(value)))
  *         postdata = "&".join(postdata)             # <<<<<<<<<<<<<<
  *         b_string = postdata.encode("utf8")
  *         qdata.postdata = strdup(b_string)
  */
-    __pyx_t_3 = __Pyx_PyString_Join(__pyx_kp_s__13, __pyx_v_postdata); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 556, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyString_Join(__pyx_kp_s__13, __pyx_v_postdata); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 558, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF_SET(__pyx_v_postdata, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "_curly.pyx":557
+    /* "_curly.pyx":559
  *             postdata.append("{}={}".format(quote(key), quote(value)))
  *         postdata = "&".join(postdata)
  *         b_string = postdata.encode("utf8")             # <<<<<<<<<<<<<<
  *         qdata.postdata = strdup(b_string)
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_postdata, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 557, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_postdata, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 559, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_13 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_13)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_13);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_13) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_13, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_s_utf8);
     __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 557, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 559, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 557, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 559, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_b_string, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "_curly.pyx":558
+    /* "_curly.pyx":560
  *         postdata = "&".join(postdata)
  *         b_string = postdata.encode("utf8")
  *         qdata.postdata = strdup(b_string)             # <<<<<<<<<<<<<<
  * 
  *     if data is not None:
  */
     if (unlikely(__pyx_v_b_string == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-      __PYX_ERR(0, 558, __pyx_L1_error)
+      __PYX_ERR(0, 560, __pyx_L1_error)
     }
-    __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 558, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 560, __pyx_L1_error)
     __pyx_v_qdata->postdata = strdup(__pyx_t_15);
 
-    /* "_curly.pyx":550
+    /* "_curly.pyx":552
  *         qdata.postdata = strdup(b_string)
  *         headers["Content-Type"] = "application/json"
  *     elif isinstance(data, dict):             # <<<<<<<<<<<<<<
  *         # XXX support multipart form-data, using curl_mime
  *         postdata = []
  */
   }
   __pyx_L12:;
 
-  /* "_curly.pyx":560
+  /* "_curly.pyx":562
  *         qdata.postdata = strdup(b_string)
  * 
  *     if data is not None:             # <<<<<<<<<<<<<<
  *         if isinstance(data, bytes):
  *             b_string = data
  */
   __pyx_t_2 = (__pyx_v_data != Py_None);
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "_curly.pyx":561
+    /* "_curly.pyx":563
  * 
  *     if data is not None:
  *         if isinstance(data, bytes):             # <<<<<<<<<<<<<<
  *             b_string = data
  *         else:
  */
     __pyx_t_1 = PyBytes_Check(__pyx_v_data); 
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (__pyx_t_2) {
 
-      /* "_curly.pyx":562
+      /* "_curly.pyx":564
  *     if data is not None:
  *         if isinstance(data, bytes):
  *             b_string = data             # <<<<<<<<<<<<<<
  *         else:
  *             b_string = data.encode("utf8")
  */
-      if (!(likely(PyBytes_CheckExact(__pyx_v_data))||((__pyx_v_data) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_data)->tp_name), 0))) __PYX_ERR(0, 562, __pyx_L1_error)
+      if (!(likely(PyBytes_CheckExact(__pyx_v_data))||((__pyx_v_data) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_data)->tp_name), 0))) __PYX_ERR(0, 564, __pyx_L1_error)
       __pyx_t_3 = __pyx_v_data;
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_DECREF_SET(__pyx_v_b_string, ((PyObject*)__pyx_t_3));
       __pyx_t_3 = 0;
 
-      /* "_curly.pyx":561
+      /* "_curly.pyx":563
  * 
  *     if data is not None:
  *         if isinstance(data, bytes):             # <<<<<<<<<<<<<<
  *             b_string = data
  *         else:
  */
       goto __pyx_L18;
     }
 
-    /* "_curly.pyx":564
+    /* "_curly.pyx":566
  *             b_string = data
  *         else:
  *             b_string = data.encode("utf8")             # <<<<<<<<<<<<<<
  *         qdata.postdata = strdup(b_string)
  * 
  */
     /*else*/ {
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 564, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 566, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_13 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_13)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_13);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_3 = (__pyx_t_13) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_13, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_s_utf8);
       __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 564, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 566, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 564, __pyx_L1_error)
+      if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 566, __pyx_L1_error)
       __Pyx_DECREF_SET(__pyx_v_b_string, ((PyObject*)__pyx_t_3));
       __pyx_t_3 = 0;
     }
     __pyx_L18:;
 
-    /* "_curly.pyx":565
+    /* "_curly.pyx":567
  *         else:
  *             b_string = data.encode("utf8")
  *         qdata.postdata = strdup(b_string)             # <<<<<<<<<<<<<<
  * 
  *     # cache
  */
     if (unlikely(__pyx_v_b_string == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-      __PYX_ERR(0, 565, __pyx_L1_error)
+      __PYX_ERR(0, 567, __pyx_L1_error)
     }
-    __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 565, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 567, __pyx_L1_error)
     __pyx_v_qdata->postdata = strdup(__pyx_t_15);
 
-    /* "_curly.pyx":560
+    /* "_curly.pyx":562
  *         qdata.postdata = strdup(b_string)
  * 
  *     if data is not None:             # <<<<<<<<<<<<<<
  *         if isinstance(data, bytes):
  *             b_string = data
  */
   }
 
-  /* "_curly.pyx":568
+  /* "_curly.pyx":570
  * 
  *     # cache
  *     if cache_fn is not None:             # <<<<<<<<<<<<<<
  *         cache_dir = dirname(cache_fn)
  *         if not exists(cache_dir):
  */
   __pyx_t_2 = (__pyx_v_cache_fn != Py_None);
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "_curly.pyx":569
+    /* "_curly.pyx":571
  *     # cache
  *     if cache_fn is not None:
  *         cache_dir = dirname(cache_fn)             # <<<<<<<<<<<<<<
  *         if not exists(cache_dir):
  *             makedirs(cache_dir)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_dirname); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 569, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_dirname); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 571, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_13 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_13)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_13);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_13) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_13, __pyx_v_cache_fn) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_cache_fn);
     __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 571, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_cache_dir = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "_curly.pyx":570
+    /* "_curly.pyx":572
  *     if cache_fn is not None:
  *         cache_dir = dirname(cache_fn)
  *         if not exists(cache_dir):             # <<<<<<<<<<<<<<
  *             makedirs(cache_dir)
  *         b_string = cache_fn.encode("utf8")
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_exists); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 570, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_exists); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_13 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_13)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_13);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_13) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_13, __pyx_v_cache_dir) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_cache_dir);
     __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 570, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 570, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 572, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_2 = ((!__pyx_t_1) != 0);
     if (__pyx_t_2) {
 
-      /* "_curly.pyx":571
+      /* "_curly.pyx":573
  *         cache_dir = dirname(cache_fn)
  *         if not exists(cache_dir):
  *             makedirs(cache_dir)             # <<<<<<<<<<<<<<
  *         b_string = cache_fn.encode("utf8")
  *         qdata.cache_fn = strdup(b_string)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_makedirs); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 571, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_makedirs); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 573, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_13 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_13)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_13);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_3 = (__pyx_t_13) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_13, __pyx_v_cache_dir) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_cache_dir);
       __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 571, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 573, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "_curly.pyx":570
+      /* "_curly.pyx":572
  *     if cache_fn is not None:
  *         cache_dir = dirname(cache_fn)
  *         if not exists(cache_dir):             # <<<<<<<<<<<<<<
  *             makedirs(cache_dir)
  *         b_string = cache_fn.encode("utf8")
  */
     }
 
-    /* "_curly.pyx":572
+    /* "_curly.pyx":574
  *         if not exists(cache_dir):
  *             makedirs(cache_dir)
  *         b_string = cache_fn.encode("utf8")             # <<<<<<<<<<<<<<
  *         qdata.cache_fn = strdup(b_string)
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_cache_fn, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 572, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_cache_fn, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 574, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_13 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_13)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_13);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_13) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_13, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_s_utf8);
     __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 572, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 574, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 572, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 574, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_b_string, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "_curly.pyx":573
+    /* "_curly.pyx":575
  *             makedirs(cache_dir)
  *         b_string = cache_fn.encode("utf8")
  *         qdata.cache_fn = strdup(b_string)             # <<<<<<<<<<<<<<
  * 
  *     # headers
  */
     if (unlikely(__pyx_v_b_string == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-      __PYX_ERR(0, 573, __pyx_L1_error)
+      __PYX_ERR(0, 575, __pyx_L1_error)
     }
-    __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 573, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 575, __pyx_L1_error)
     __pyx_v_qdata->cache_fn = strdup(__pyx_t_15);
 
-    /* "_curly.pyx":568
+    /* "_curly.pyx":570
  * 
  *     # cache
  *     if cache_fn is not None:             # <<<<<<<<<<<<<<
  *         cache_dir = dirname(cache_fn)
  *         if not exists(cache_dir):
  */
   }
 
-  /* "_curly.pyx":576
+  /* "_curly.pyx":578
  * 
  *     # headers
  *     if headers is not None:             # <<<<<<<<<<<<<<
  *         for key, value in headers.iteritems():
  *             header = "{}: {}".format(key, value).encode("utf8")
  */
   __pyx_t_2 = (__pyx_v_headers != Py_None);
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "_curly.pyx":577
+    /* "_curly.pyx":579
  *     # headers
  *     if headers is not None:
  *         for key, value in headers.iteritems():             # <<<<<<<<<<<<<<
  *             header = "{}: {}".format(key, value).encode("utf8")
  *             c_header = header
  */
     __pyx_t_7 = 0;
     if (unlikely(__pyx_v_headers == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "iteritems");
-      __PYX_ERR(0, 577, __pyx_L1_error)
+      __PYX_ERR(0, 579, __pyx_L1_error)
     }
-    __pyx_t_5 = __Pyx_dict_iterator(__pyx_v_headers, 0, __pyx_n_s_iteritems, (&__pyx_t_16), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 577, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_dict_iterator(__pyx_v_headers, 0, __pyx_n_s_iteritems, (&__pyx_t_16), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_5;
     __pyx_t_5 = 0;
     while (1) {
       __pyx_t_17 = __Pyx_dict_iter_next(__pyx_t_3, __pyx_t_16, &__pyx_t_7, &__pyx_t_5, &__pyx_t_13, NULL, __pyx_t_4);
       if (unlikely(__pyx_t_17 == 0)) break;
-      if (unlikely(__pyx_t_17 == -1)) __PYX_ERR(0, 577, __pyx_L1_error)
+      if (unlikely(__pyx_t_17 == -1)) __PYX_ERR(0, 579, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_5);
       __pyx_t_5 = 0;
       __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_13);
       __pyx_t_13 = 0;
 
-      /* "_curly.pyx":578
+      /* "_curly.pyx":580
  *     if headers is not None:
  *         for key, value in headers.iteritems():
  *             header = "{}: {}".format(key, value).encode("utf8")             # <<<<<<<<<<<<<<
  *             c_header = header
  *             qdata.headers = curl_slist_append(
  */
-      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__14, __pyx_n_s_format); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 578, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__14, __pyx_n_s_format); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 580, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       __pyx_t_10 = NULL;
       __pyx_t_17 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_12);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
@@ -9414,134 +9554,134 @@
           __Pyx_DECREF_SET(__pyx_t_12, function);
           __pyx_t_17 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_12)) {
         PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_v_key, __pyx_v_value};
-        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_17, 2+__pyx_t_17); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 578, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_17, 2+__pyx_t_17); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 580, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_GOTREF(__pyx_t_5);
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_12)) {
         PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_v_key, __pyx_v_value};
-        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_17, 2+__pyx_t_17); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 578, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_17, 2+__pyx_t_17); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 580, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_GOTREF(__pyx_t_5);
       } else
       #endif
       {
-        __pyx_t_9 = PyTuple_New(2+__pyx_t_17); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 578, __pyx_L1_error)
+        __pyx_t_9 = PyTuple_New(2+__pyx_t_17); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 580, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         if (__pyx_t_10) {
           __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_10); __pyx_t_10 = NULL;
         }
         __Pyx_INCREF(__pyx_v_key);
         __Pyx_GIVEREF(__pyx_v_key);
         PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_17, __pyx_v_key);
         __Pyx_INCREF(__pyx_v_value);
         __Pyx_GIVEREF(__pyx_v_value);
         PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_17, __pyx_v_value);
-        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_9, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 578, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_9, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 580, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_encode); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 578, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_encode); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 580, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_12);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_12, function);
         }
       }
       __pyx_t_13 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_5, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_n_s_utf8);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 578, __pyx_L1_error)
+      if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 580, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_XDECREF_SET(__pyx_v_header, __pyx_t_13);
       __pyx_t_13 = 0;
 
-      /* "_curly.pyx":579
+      /* "_curly.pyx":581
  *         for key, value in headers.iteritems():
  *             header = "{}: {}".format(key, value).encode("utf8")
  *             c_header = header             # <<<<<<<<<<<<<<
  *             qdata.headers = curl_slist_append(
  *                 qdata.headers, c_header)
  */
-      __pyx_t_18 = __Pyx_PyObject_AsWritableString(__pyx_v_header); if (unlikely((!__pyx_t_18) && PyErr_Occurred())) __PYX_ERR(0, 579, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyObject_AsWritableString(__pyx_v_header); if (unlikely((!__pyx_t_18) && PyErr_Occurred())) __PYX_ERR(0, 581, __pyx_L1_error)
       __pyx_v_c_header = __pyx_t_18;
 
-      /* "_curly.pyx":580
+      /* "_curly.pyx":582
  *             header = "{}: {}".format(key, value).encode("utf8")
  *             c_header = header
  *             qdata.headers = curl_slist_append(             # <<<<<<<<<<<<<<
  *                 qdata.headers, c_header)
  * 
  */
       __pyx_v_qdata->headers = curl_slist_append(__pyx_v_qdata->headers, __pyx_v_c_header);
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "_curly.pyx":576
+    /* "_curly.pyx":578
  * 
  *     # headers
  *     if headers is not None:             # <<<<<<<<<<<<<<
  *         for key, value in headers.iteritems():
  *             header = "{}: {}".format(key, value).encode("utf8")
  */
   }
 
-  /* "_curly.pyx":584
+  /* "_curly.pyx":586
  * 
  *     # callback
  *     if callback is not None:             # <<<<<<<<<<<<<<
  *         qdata.callback = <void *>callback
  *         Py_XINCREF(<PyObject *>qdata.callback)
  */
   __pyx_t_1 = (__pyx_v_callback != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "_curly.pyx":585
+    /* "_curly.pyx":587
  *     # callback
  *     if callback is not None:
  *         qdata.callback = <void *>callback             # <<<<<<<<<<<<<<
  *         Py_XINCREF(<PyObject *>qdata.callback)
  * 
  */
     __pyx_v_qdata->callback = ((void *)__pyx_v_callback);
 
-    /* "_curly.pyx":586
+    /* "_curly.pyx":588
  *     if callback is not None:
  *         qdata.callback = <void *>callback
  *         Py_XINCREF(<PyObject *>qdata.callback)             # <<<<<<<<<<<<<<
  * 
  *     # auth
  */
     Py_XINCREF(((PyObject *)__pyx_v_qdata->callback));
 
-    /* "_curly.pyx":584
+    /* "_curly.pyx":586
  * 
  *     # callback
  *     if callback is not None:             # <<<<<<<<<<<<<<
  *         qdata.callback = <void *>callback
  *         Py_XINCREF(<PyObject *>qdata.callback)
  */
   }
 
-  /* "_curly.pyx":589
+  /* "_curly.pyx":591
  * 
  *     # auth
  *     if isinstance(auth, (tuple, list)):             # <<<<<<<<<<<<<<
  *         # supports HTTP AUTH
  *         obj = "{}:{}".format(*auth)
  */
   __pyx_t_1 = PyTuple_Check(__pyx_v_auth); 
@@ -9554,182 +9694,182 @@
   __pyx_t_19 = PyList_Check(__pyx_v_auth); 
   __pyx_t_1 = (__pyx_t_19 != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L26_bool_binop_done:;
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "_curly.pyx":591
+    /* "_curly.pyx":593
  *     if isinstance(auth, (tuple, list)):
  *         # supports HTTP AUTH
  *         obj = "{}:{}".format(*auth)             # <<<<<<<<<<<<<<
  *         b_string = obj.encode("utf8")
  *         qdata.auth_userpwd = strdup(b_string)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__15, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 591, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__15, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 593, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_13 = __Pyx_PySequence_Tuple(__pyx_v_auth); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 591, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PySequence_Tuple(__pyx_v_auth); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 593, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
-    __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_13, NULL); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 591, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_13, NULL); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 593, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     __pyx_v_obj = __pyx_t_12;
     __pyx_t_12 = 0;
 
-    /* "_curly.pyx":592
+    /* "_curly.pyx":594
  *         # supports HTTP AUTH
  *         obj = "{}:{}".format(*auth)
  *         b_string = obj.encode("utf8")             # <<<<<<<<<<<<<<
  *         qdata.auth_userpwd = strdup(b_string)
  *     elif auth is None:
  */
-    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_obj, __pyx_n_s_encode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_obj, __pyx_n_s_encode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 594, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_13);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_13, function);
       }
     }
     __pyx_t_12 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_3, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_n_s_utf8);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 592, __pyx_L1_error)
+    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 594, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_12))||((__pyx_t_12) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_12)->tp_name), 0))) __PYX_ERR(0, 592, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_12))||((__pyx_t_12) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_12)->tp_name), 0))) __PYX_ERR(0, 594, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_b_string, ((PyObject*)__pyx_t_12));
     __pyx_t_12 = 0;
 
-    /* "_curly.pyx":593
+    /* "_curly.pyx":595
  *         obj = "{}:{}".format(*auth)
  *         b_string = obj.encode("utf8")
  *         qdata.auth_userpwd = strdup(b_string)             # <<<<<<<<<<<<<<
  *     elif auth is None:
  *         pass
  */
     if (unlikely(__pyx_v_b_string == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-      __PYX_ERR(0, 593, __pyx_L1_error)
+      __PYX_ERR(0, 595, __pyx_L1_error)
     }
-    __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 593, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 595, __pyx_L1_error)
     __pyx_v_qdata->auth_userpwd = strdup(__pyx_t_15);
 
-    /* "_curly.pyx":589
+    /* "_curly.pyx":591
  * 
  *     # auth
  *     if isinstance(auth, (tuple, list)):             # <<<<<<<<<<<<<<
  *         # supports HTTP AUTH
  *         obj = "{}:{}".format(*auth)
  */
     goto __pyx_L25;
   }
 
-  /* "_curly.pyx":594
+  /* "_curly.pyx":596
  *         b_string = obj.encode("utf8")
  *         qdata.auth_userpwd = strdup(b_string)
  *     elif auth is None:             # <<<<<<<<<<<<<<
  *         pass
  *     else:
  */
   __pyx_t_1 = (__pyx_v_auth == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (likely(__pyx_t_2)) {
     goto __pyx_L25;
   }
 
-  /* "_curly.pyx":597
+  /* "_curly.pyx":599
  *         pass
  *     else:
  *         dl_queue_node_free(&qdata)             # <<<<<<<<<<<<<<
  *         raise Exception("Unsupported auth for the moment")
  * 
  */
   /*else*/ {
     __pyx_f_6_curly_dl_queue_node_free((&__pyx_v_qdata));
 
-    /* "_curly.pyx":598
+    /* "_curly.pyx":600
  *     else:
  *         dl_queue_node_free(&qdata)
  *         raise Exception("Unsupported auth for the moment")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_12 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 598, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 600, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_Raise(__pyx_t_12, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __PYX_ERR(0, 598, __pyx_L1_error)
+    __PYX_ERR(0, 600, __pyx_L1_error)
   }
   __pyx_L25:;
 
-  /* "_curly.pyx":601
+  /* "_curly.pyx":603
  * 
  * 
  *     dl_ensure_init()             # <<<<<<<<<<<<<<
  *     if priority:
  *         queue_append_first(&ctx_download, qdata)
  */
   __pyx_f_6_curly_dl_ensure_init();
 
-  /* "_curly.pyx":602
+  /* "_curly.pyx":604
  * 
  *     dl_ensure_init()
  *     if priority:             # <<<<<<<<<<<<<<
  *         queue_append_first(&ctx_download, qdata)
  *     else:
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_priority); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 602, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_priority); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 604, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "_curly.pyx":603
+    /* "_curly.pyx":605
  *     dl_ensure_init()
  *     if priority:
  *         queue_append_first(&ctx_download, qdata)             # <<<<<<<<<<<<<<
  *     else:
  *         queue_append_last(&ctx_download, qdata)
  */
     (void)(__pyx_f_6_curly_queue_append_first((&__pyx_v_6_curly_ctx_download), __pyx_v_qdata));
 
-    /* "_curly.pyx":602
+    /* "_curly.pyx":604
  * 
  *     dl_ensure_init()
  *     if priority:             # <<<<<<<<<<<<<<
  *         queue_append_first(&ctx_download, qdata)
  *     else:
  */
     goto __pyx_L28;
   }
 
-  /* "_curly.pyx":605
+  /* "_curly.pyx":607
  *         queue_append_first(&ctx_download, qdata)
  *     else:
  *         queue_append_last(&ctx_download, qdata)             # <<<<<<<<<<<<<<
  *     SDL_SemPost(dl_sem)
  * 
  */
   /*else*/ {
     (void)(__pyx_f_6_curly_queue_append_last((&__pyx_v_6_curly_ctx_download), __pyx_v_qdata));
   }
   __pyx_L28:;
 
-  /* "_curly.pyx":606
+  /* "_curly.pyx":608
  *     else:
  *         queue_append_last(&ctx_download, qdata)
  *     SDL_SemPost(dl_sem)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(SDL_SemPost(__pyx_v_6_curly_dl_sem));
 
-  /* "_curly.pyx":464
+  /* "_curly.pyx":466
  * 
  * 
  * def request(url, callback, headers=None,             # <<<<<<<<<<<<<<
  *             method="GET", params=None, data=None, json=None,
  *             auth=None, cache_fn=None, preload_image=False,
  */
 
@@ -9758,15 +9898,15 @@
   __Pyx_XDECREF(__pyx_v_url);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":609
+/* "_curly.pyx":611
  * 
  * 
  * def download_image(*args, **kwargs):             # <<<<<<<<<<<<<<
  *     """A wrapper around :func:`request` that set `preload_image` to True
  *     """
  */
 
@@ -9795,65 +9935,70 @@
 }
 
 static PyObject *__pyx_pf_6_curly_4download_image(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("download_image", 0);
 
-  /* "_curly.pyx":612
+  /* "_curly.pyx":614
  *     """A wrapper around :func:`request` that set `preload_image` to True
  *     """
  *     kwargs["preload_image"] = True             # <<<<<<<<<<<<<<
  *     request(*args, **kwargs)
  * 
  */
-  if (unlikely(PyDict_SetItem(__pyx_v_kwargs, __pyx_n_s_preload_image, Py_True) < 0)) __PYX_ERR(0, 612, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_kwargs, __pyx_n_s_preload_image, Py_True) < 0)) __PYX_ERR(0, 614, __pyx_L1_error)
 
-  /* "_curly.pyx":613
+  /* "_curly.pyx":615
  *     """
  *     kwargs["preload_image"] = True
  *     request(*args, **kwargs)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_request); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 613, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_request); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 615, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_v_args, __pyx_v_kwargs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 613, __pyx_L1_error)
+  __pyx_t_2 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 615, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_v_args, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 615, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "_curly.pyx":609
+  /* "_curly.pyx":611
  * 
  * 
  * def download_image(*args, **kwargs):             # <<<<<<<<<<<<<<
  *     """A wrapper around :func:`request` that set `preload_image` to True
  *     """
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("_curly.download_image", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":616
+/* "_curly.pyx":618
  * 
  * 
  * def process(*args):             # <<<<<<<<<<<<<<
  *     """Process results. It must be called as must as possible in order
  *     to process the results from the download threads.
  */
 
@@ -9890,135 +10035,135 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("process", 0);
 
-  /* "_curly.pyx":626
+  /* "_curly.pyx":628
  *         CurlyResult result
  *         dl_queue_data *data
  *         bytes b_data = None             # <<<<<<<<<<<<<<
  *         object callback
  *         curl_slist *item
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_b_data = ((PyObject*)Py_None);
 
-  /* "_curly.pyx":630
+  /* "_curly.pyx":632
  *         curl_slist *item
  * 
  *     while SDL_AtomicDecRef(&dl_ready_to_process) == 0:             # <<<<<<<<<<<<<<
  *         data = <dl_queue_data *>queue_pop_first(&ctx_result)
  *         if data == NULL:
  */
   while (1) {
     __pyx_t_1 = ((SDL_AtomicDecRef((&__pyx_v_6_curly_dl_ready_to_process)) == 0) != 0);
     if (!__pyx_t_1) break;
 
-    /* "_curly.pyx":631
+    /* "_curly.pyx":633
  * 
  *     while SDL_AtomicDecRef(&dl_ready_to_process) == 0:
  *         data = <dl_queue_data *>queue_pop_first(&ctx_result)             # <<<<<<<<<<<<<<
  *         if data == NULL:
  *             break
  */
     __pyx_v_data = ((__pyx_t_6_curly_dl_queue_data *)__pyx_f_6_curly_queue_pop_first((&__pyx_v_6_curly_ctx_result)));
 
-    /* "_curly.pyx":632
+    /* "_curly.pyx":634
  *     while SDL_AtomicDecRef(&dl_ready_to_process) == 0:
  *         data = <dl_queue_data *>queue_pop_first(&ctx_result)
  *         if data == NULL:             # <<<<<<<<<<<<<<
  *             break
  * 
  */
     __pyx_t_1 = ((__pyx_v_data == NULL) != 0);
     if (__pyx_t_1) {
 
-      /* "_curly.pyx":633
+      /* "_curly.pyx":635
  *         data = <dl_queue_data *>queue_pop_first(&ctx_result)
  *         if data == NULL:
  *             break             # <<<<<<<<<<<<<<
  * 
  *         callback = <object><void *>data.callback
  */
       goto __pyx_L4_break;
 
-      /* "_curly.pyx":632
+      /* "_curly.pyx":634
  *     while SDL_AtomicDecRef(&dl_ready_to_process) == 0:
  *         data = <dl_queue_data *>queue_pop_first(&ctx_result)
  *         if data == NULL:             # <<<<<<<<<<<<<<
  *             break
  * 
  */
     }
 
-    /* "_curly.pyx":635
+    /* "_curly.pyx":637
  *             break
  * 
  *         callback = <object><void *>data.callback             # <<<<<<<<<<<<<<
  *         if not callback:
  *             continue
  */
     __pyx_t_2 = ((PyObject *)((void *)__pyx_v_data->callback));
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_callback, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "_curly.pyx":636
+    /* "_curly.pyx":638
  * 
  *         callback = <object><void *>data.callback
  *         if not callback:             # <<<<<<<<<<<<<<
  *             continue
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_callback); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 636, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_callback); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 638, __pyx_L1_error)
     __pyx_t_3 = ((!__pyx_t_1) != 0);
     if (__pyx_t_3) {
 
-      /* "_curly.pyx":637
+      /* "_curly.pyx":639
  *         callback = <object><void *>data.callback
  *         if not callback:
  *             continue             # <<<<<<<<<<<<<<
  * 
  *         result = CurlyResult()
  */
       goto __pyx_L3_continue;
 
-      /* "_curly.pyx":636
+      /* "_curly.pyx":638
  * 
  *         callback = <object><void *>data.callback
  *         if not callback:             # <<<<<<<<<<<<<<
  *             continue
  * 
  */
     }
 
-    /* "_curly.pyx":639
+    /* "_curly.pyx":641
  *             continue
  * 
  *         result = CurlyResult()             # <<<<<<<<<<<<<<
  *         result._data = data
  *         callback(result)
  */
-    __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_6_curly_CurlyResult)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 639, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_6_curly_CurlyResult)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 641, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_result, ((struct __pyx_obj_6_curly_CurlyResult *)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "_curly.pyx":640
+    /* "_curly.pyx":642
  * 
  *         result = CurlyResult()
  *         result._data = data             # <<<<<<<<<<<<<<
  *         callback(result)
  * 
  */
     __pyx_v_result->_data = __pyx_v_data;
 
-    /* "_curly.pyx":641
+    /* "_curly.pyx":643
  *         result = CurlyResult()
  *         result._data = data
  *         callback(result)             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __Pyx_INCREF(__pyx_v_callback);
@@ -10030,23 +10175,23 @@
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, ((PyObject *)__pyx_v_result)) : __Pyx_PyObject_CallOneArg(__pyx_t_4, ((PyObject *)__pyx_v_result));
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 641, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 643, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_L3_continue:;
   }
   __pyx_L4_break:;
 
-  /* "_curly.pyx":616
+  /* "_curly.pyx":618
  * 
  * 
  * def process(*args):             # <<<<<<<<<<<<<<
  *     """Process results. It must be called as must as possible in order
  *     to process the results from the download threads.
  */
 
@@ -10064,15 +10209,15 @@
   __Pyx_XDECREF(__pyx_v_b_data);
   __Pyx_XDECREF(__pyx_v_callback);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":644
+/* "_curly.pyx":646
  * 
  * 
  * def install():             # <<<<<<<<<<<<<<
  *     """Install a scheduler in the Kivy clock to call :func:`process`
  *     """
  */
 
@@ -10102,55 +10247,55 @@
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("install", 0);
 
-  /* "_curly.pyx":647
+  /* "_curly.pyx":649
  *     """Install a scheduler in the Kivy clock to call :func:`process`
  *     """
  *     uninstall()             # <<<<<<<<<<<<<<
  *     Clock.schedule_interval(process, 1 / 120.)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_uninstall); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 647, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_uninstall); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 649, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 647, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 649, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_curly.pyx":648
+  /* "_curly.pyx":650
  *     """
  *     uninstall()
  *     Clock.schedule_interval(process, 1 / 120.)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Clock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 648, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Clock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_schedule_interval); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 648, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_schedule_interval); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_process); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 648, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_process); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyFloat_FromDouble((1.0 / 120.)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 648, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble((1.0 / 120.)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -10159,51 +10304,51 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_2, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 648, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 650, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_2, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 648, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 650, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 648, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 650, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
     __pyx_t_2 = 0;
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 648, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 650, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_curly.pyx":644
+  /* "_curly.pyx":646
  * 
  * 
  * def install():             # <<<<<<<<<<<<<<
  *     """Install a scheduler in the Kivy clock to call :func:`process`
  *     """
  */
 
@@ -10221,15 +10366,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":651
+/* "_curly.pyx":653
  * 
  * 
  * def uninstall():             # <<<<<<<<<<<<<<
  *     """Uninstall the scheduler that call :func:`process` from the Kivy clock
  *     """
  */
 
@@ -10256,47 +10401,47 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("uninstall", 0);
 
-  /* "_curly.pyx":654
+  /* "_curly.pyx":656
  *     """Uninstall the scheduler that call :func:`process` from the Kivy clock
  *     """
  *     Clock.unschedule(process)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Clock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 654, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Clock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 656, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_unschedule); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 654, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_unschedule); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 656, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_process); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 654, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_process); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 656, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 654, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 656, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_curly.pyx":651
+  /* "_curly.pyx":653
  * 
  * 
  * def uninstall():             # <<<<<<<<<<<<<<
  *     """Uninstall the scheduler that call :func:`process` from the Kivy clock
  *     """
  */
 
@@ -10312,15 +10457,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":657
+/* "_curly.pyx":659
  * 
  * 
  * def stop():             # <<<<<<<<<<<<<<
  *     """Stop any threads working in the background.
  *     Any ongoing results or request will be stopped.
  */
 
@@ -10346,68 +10491,68 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("stop", 0);
 
-  /* "_curly.pyx":661
+  /* "_curly.pyx":663
  *     Any ongoing results or request will be stopped.
  *     """
  *     uninstall()             # <<<<<<<<<<<<<<
  *     SDL_AtomicSet(&dl_done, 1)
  *     SDL_SemPost(dl_sem)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_uninstall); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 661, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_uninstall); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 661, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_curly.pyx":662
+  /* "_curly.pyx":664
  *     """
  *     uninstall()
  *     SDL_AtomicSet(&dl_done, 1)             # <<<<<<<<<<<<<<
  *     SDL_SemPost(dl_sem)
  *     SDL_DestroySemaphore(dl_sem)
  */
   (void)(SDL_AtomicSet((&__pyx_v_6_curly_dl_done), 1));
 
-  /* "_curly.pyx":663
+  /* "_curly.pyx":665
  *     uninstall()
  *     SDL_AtomicSet(&dl_done, 1)
  *     SDL_SemPost(dl_sem)             # <<<<<<<<<<<<<<
  *     SDL_DestroySemaphore(dl_sem)
  * 
  */
   (void)(SDL_SemPost(__pyx_v_6_curly_dl_sem));
 
-  /* "_curly.pyx":664
+  /* "_curly.pyx":666
  *     SDL_AtomicSet(&dl_done, 1)
  *     SDL_SemPost(dl_sem)
  *     SDL_DestroySemaphore(dl_sem)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   SDL_DestroySemaphore(__pyx_v_6_curly_dl_sem);
 
-  /* "_curly.pyx":657
+  /* "_curly.pyx":659
  * 
  * 
  * def stop():             # <<<<<<<<<<<<<<
  *     """Stop any threads working in the background.
  *     Any ongoing results or request will be stopped.
  */
 
@@ -10422,44 +10567,48 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_curly.pyx":667
+/* "_curly.pyx":669
  * 
  * 
- * def configure(num_threads=4, req_verify_peer=0):             # <<<<<<<<<<<<<<
+ * def configure(num_threads=4, req_verify_peer=0, useragent=None):             # <<<<<<<<<<<<<<
  *     """Configure the library before any invocation
  *     Any call after the using `request`, `download_image` or `get_info`
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6_curly_15configure(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6_curly_14configure[] = "Configure the library before any invocation\n    Any call after the using `request`, `download_image` or `get_info`\n    won't use the information and raise an exception.\n\n    :Parameters:\n        `num_threads`: int\n            Number of background threads to use for downloading\n            Defaults to 4\n        `req_verify_peer`: bool\n            If True, it will verify SSL peers.\n            But since we have an issue with cacert.pem on Android, it is\n            disabled by default right now. (it's bad)\n            Defaults to False\n    ";
 static PyMethodDef __pyx_mdef_6_curly_15configure = {"configure", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6_curly_15configure, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6_curly_14configure};
 static PyObject *__pyx_pw_6_curly_15configure(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_num_threads = 0;
   PyObject *__pyx_v_req_verify_peer = 0;
+  PyObject *__pyx_v_useragent = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("configure (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_num_threads,&__pyx_n_s_req_verify_peer,0};
-    PyObject* values[2] = {0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_num_threads,&__pyx_n_s_req_verify_peer,&__pyx_n_s_useragent,0};
+    PyObject* values[3] = {0,0,0};
     values[0] = ((PyObject *)__pyx_int_4);
     values[1] = ((PyObject *)__pyx_int_0);
+    values[2] = ((PyObject *)Py_None);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
@@ -10472,127 +10621,207 @@
         }
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_req_verify_peer);
           if (value) { values[1] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_useragent);
+          if (value) { values[2] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "configure") < 0)) __PYX_ERR(0, 667, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "configure") < 0)) __PYX_ERR(0, 669, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_num_threads = values[0];
     __pyx_v_req_verify_peer = values[1];
+    __pyx_v_useragent = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("configure", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 667, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("configure", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 669, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_curly.configure", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6_curly_14configure(__pyx_self, __pyx_v_num_threads, __pyx_v_req_verify_peer);
+  __pyx_r = __pyx_pf_6_curly_14configure(__pyx_self, __pyx_v_num_threads, __pyx_v_req_verify_peer, __pyx_v_useragent);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6_curly_14configure(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_num_threads, PyObject *__pyx_v_req_verify_peer) {
+static PyObject *__pyx_pf_6_curly_14configure(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_num_threads, PyObject *__pyx_v_req_verify_peer, PyObject *__pyx_v_useragent) {
+  PyObject *__pyx_v_b_string = 0;
+  CYTHON_UNUSED char *__pyx_v_config_useragent;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  char const *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("configure", 0);
 
-  /* "_curly.pyx":682
+  /* "_curly.pyx":684
  *             Defaults to False
  *     """
  *     if dl_running:             # <<<<<<<<<<<<<<
  *         raise Exception("Library already running, cannot reconfigure.")
  *     global config_num_threads, config_req_verify_peer
  */
   __pyx_t_1 = (__pyx_v_6_curly_dl_running != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "_curly.pyx":683
+    /* "_curly.pyx":685
  *     """
  *     if dl_running:
  *         raise Exception("Library already running, cannot reconfigure.")             # <<<<<<<<<<<<<<
  *     global config_num_threads, config_req_verify_peer
  *     config_num_threads = num_threads
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 683, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 685, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 683, __pyx_L1_error)
+    __PYX_ERR(0, 685, __pyx_L1_error)
 
-    /* "_curly.pyx":682
+    /* "_curly.pyx":684
  *             Defaults to False
  *     """
  *     if dl_running:             # <<<<<<<<<<<<<<
  *         raise Exception("Library already running, cannot reconfigure.")
  *     global config_num_threads, config_req_verify_peer
  */
   }
 
-  /* "_curly.pyx":685
+  /* "_curly.pyx":687
  *         raise Exception("Library already running, cannot reconfigure.")
  *     global config_num_threads, config_req_verify_peer
  *     config_num_threads = num_threads             # <<<<<<<<<<<<<<
  *     config_req_verify_peer = 1 if req_verify_peer else 0
+ * 
  */
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_num_threads); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 685, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_num_threads); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 687, __pyx_L1_error)
   __pyx_v_6_curly_config_num_threads = __pyx_t_3;
 
-  /* "_curly.pyx":686
+  /* "_curly.pyx":688
  *     global config_num_threads, config_req_verify_peer
  *     config_num_threads = num_threads
  *     config_req_verify_peer = 1 if req_verify_peer else 0             # <<<<<<<<<<<<<<
+ * 
+ *     cdef bytes b_string
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_req_verify_peer); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 686, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_req_verify_peer); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 688, __pyx_L1_error)
   if (__pyx_t_1) {
     __pyx_t_3 = 1;
   } else {
     __pyx_t_3 = 0;
   }
   __pyx_v_6_curly_config_req_verify_peer = __pyx_t_3;
 
-  /* "_curly.pyx":667
+  /* "_curly.pyx":691
  * 
+ *     cdef bytes b_string
+ *     if useragent:             # <<<<<<<<<<<<<<
+ *         b_string = useragent.encode("utf8")
+ *         config_useragent = strdup(b_string)
+ */
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_useragent); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 691, __pyx_L1_error)
+  if (__pyx_t_1) {
+
+    /* "_curly.pyx":692
+ *     cdef bytes b_string
+ *     if useragent:
+ *         b_string = useragent.encode("utf8")             # <<<<<<<<<<<<<<
+ *         config_useragent = strdup(b_string)
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_useragent, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 692, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
+      }
+    }
+    __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_n_s_utf8);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 692, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (!(likely(PyBytes_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 692, __pyx_L1_error)
+    __pyx_v_b_string = ((PyObject*)__pyx_t_2);
+    __pyx_t_2 = 0;
+
+    /* "_curly.pyx":693
+ *     if useragent:
+ *         b_string = useragent.encode("utf8")
+ *         config_useragent = strdup(b_string)             # <<<<<<<<<<<<<<
+ * 
+ */
+    if (unlikely(__pyx_v_b_string == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
+      __PYX_ERR(0, 693, __pyx_L1_error)
+    }
+    __pyx_t_6 = __Pyx_PyBytes_AsString(__pyx_v_b_string); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 693, __pyx_L1_error)
+    __pyx_v_config_useragent = strdup(__pyx_t_6);
+
+    /* "_curly.pyx":691
+ * 
+ *     cdef bytes b_string
+ *     if useragent:             # <<<<<<<<<<<<<<
+ *         b_string = useragent.encode("utf8")
+ *         config_useragent = strdup(b_string)
+ */
+  }
+
+  /* "_curly.pyx":669
  * 
- * def configure(num_threads=4, req_verify_peer=0):             # <<<<<<<<<<<<<<
+ * 
+ * def configure(num_threads=4, req_verify_peer=0, useragent=None):             # <<<<<<<<<<<<<<
  *     """Configure the library before any invocation
  *     Any call after the using `request`, `download_image` or `get_info`
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("_curly.configure", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_b_string);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_tp_new_6_curly_CurlyResult(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_6_curly_CurlyResult *p;
@@ -10786,20 +11015,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
@@ -10888,14 +11120,15 @@
   {&__pyx_n_s_b_string, __pyx_k_b_string, sizeof(__pyx_k_b_string), 0, 0, 1, 1},
   {&__pyx_n_s_c_header, __pyx_k_c_header, sizeof(__pyx_k_c_header), 0, 0, 1, 1},
   {&__pyx_n_s_cache_dir, __pyx_k_cache_dir, sizeof(__pyx_k_cache_dir), 0, 0, 1, 1},
   {&__pyx_n_s_cache_fn, __pyx_k_cache_fn, sizeof(__pyx_k_cache_fn), 0, 0, 1, 1},
   {&__pyx_n_s_callback, __pyx_k_callback, sizeof(__pyx_k_callback), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_code, __pyx_k_code, sizeof(__pyx_k_code), 0, 0, 1, 1},
+  {&__pyx_n_s_config_useragent, __pyx_k_config_useragent, sizeof(__pyx_k_config_useragent), 0, 0, 1, 1},
   {&__pyx_n_s_configure, __pyx_k_configure, sizeof(__pyx_k_configure), 0, 0, 1, 1},
   {&__pyx_kp_s_content_type, __pyx_k_content_type, sizeof(__pyx_k_content_type), 0, 0, 1, 0},
   {&__pyx_n_s_curl_ret, __pyx_k_curl_ret, sizeof(__pyx_k_curl_ret), 0, 0, 1, 1},
   {&__pyx_n_s_curly, __pyx_k_curly, sizeof(__pyx_k_curly), 0, 0, 1, 1},
   {&__pyx_kp_s_curly__curly_pyx, __pyx_k_curly__curly_pyx, sizeof(__pyx_k_curly__curly_pyx), 0, 0, 1, 0},
   {&__pyx_kp_s_curly_requires_ssl_linked_otherw, __pyx_k_curly_requires_ssl_linked_otherw, sizeof(__pyx_k_curly_requires_ssl_linked_otherw), 0, 0, 1, 0},
   {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
@@ -10989,64 +11222,65 @@
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_uninstall, __pyx_k_uninstall, sizeof(__pyx_k_uninstall), 0, 0, 1, 1},
   {&__pyx_n_s_unschedule, __pyx_k_unschedule, sizeof(__pyx_k_unschedule), 0, 0, 1, 1},
   {&__pyx_n_s_url, __pyx_k_url, sizeof(__pyx_k_url), 0, 0, 1, 1},
   {&__pyx_n_s_url_suffix, __pyx_k_url_suffix, sizeof(__pyx_k_url_suffix), 0, 0, 1, 1},
   {&__pyx_n_s_urllib, __pyx_k_urllib, sizeof(__pyx_k_urllib), 0, 0, 1, 1},
   {&__pyx_n_s_urllib_parse, __pyx_k_urllib_parse, sizeof(__pyx_k_urllib_parse), 0, 0, 1, 1},
+  {&__pyx_n_s_useragent, __pyx_k_useragent, sizeof(__pyx_k_useragent), 0, 0, 1, 1},
   {&__pyx_n_s_utf8, __pyx_k_utf8, sizeof(__pyx_k_utf8), 0, 0, 1, 1},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {&__pyx_n_s_version, __pyx_k_version, sizeof(__pyx_k_version), 0, 0, 1, 1},
   {&__pyx_n_s_w, __pyx_k_w, sizeof(__pyx_k_w), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(0, 6, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 177, __pyx_L1_error)
-  __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 271, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "_curly.pyx":326
+  /* "_curly.pyx":328
  * 
  *         if not self._data.preload_image:
  *             raise Exception("Preload image not used")             # <<<<<<<<<<<<<<
  * 
  *         # send back an image
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_Preload_image_not_used); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_Preload_image_not_used); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 328, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "_curly.pyx":454
+  /* "_curly.pyx":456
  *         interpreted and returned
  *         """
  *         if not self.headers.get("content-type", "").startswith("application/json"):             # <<<<<<<<<<<<<<
  *             raise Exception("Not a application/json response")
  *         if self._json is None:
  */
-  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_kp_s_content_type, __pyx_kp_s_); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_kp_s_content_type, __pyx_kp_s_); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 456, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "_curly.pyx":455
+  /* "_curly.pyx":457
  *         """
  *         if not self.headers.get("content-type", "").startswith("application/json"):
  *             raise Exception("Not a application/json response")             # <<<<<<<<<<<<<<
  *         if self._json is None:
  *             self._json = loads(self.data)
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_Not_a_application_json_response); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 455, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_Not_a_application_json_response); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -11061,157 +11295,157 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "_curly.pyx":519
+  /* "_curly.pyx":521
  * 
  *     if data and json:
  *         raise Exception("Cannot have data and json parameters at the same time")             # <<<<<<<<<<<<<<
  * 
  *     # allocate qdata
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_Cannot_have_data_and_json_parame); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 519, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_Cannot_have_data_and_json_parame); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 521, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "_curly.pyx":598
+  /* "_curly.pyx":600
  *     else:
  *         dl_queue_node_free(&qdata)
  *         raise Exception("Unsupported auth for the moment")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Unsupported_auth_for_the_moment); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 598, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Unsupported_auth_for_the_moment); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "_curly.pyx":683
+  /* "_curly.pyx":685
  *     """
  *     if dl_running:
  *         raise Exception("Library already running, cannot reconfigure.")             # <<<<<<<<<<<<<<
  *     global config_num_threads, config_req_verify_peer
  *     config_num_threads = num_threads
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Library_already_running_cannot_r); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 683, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Library_already_running_cannot_r); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 685, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "_curly.pyx":191
+  /* "_curly.pyx":193
  * 
  * 
  * def get_info():             # <<<<<<<<<<<<<<
  *     cdef curl_version_info_data *info
  *     dl_ensure_init()
  */
-  __pyx_tuple__18 = PyTuple_Pack(2, __pyx_n_s_info, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(2, __pyx_n_s_info, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_get_info, 191, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_get_info, 193, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 193, __pyx_L1_error)
 
-  /* "_curly.pyx":265
+  /* "_curly.pyx":267
  * class ImageLoaderMemory(ImageLoaderBase):
  *     # Internal loader for data loaded from SDL2
  *     def __init__(self, filename, data, **kwargs):             # <<<<<<<<<<<<<<
  *         w, h, fmt, pixels, rowlength = data
  *         self._data = [ImageData(
  */
-  __pyx_tuple__20 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_filename, __pyx_n_s_data, __pyx_n_s_kwargs, __pyx_n_s_w, __pyx_n_s_h, __pyx_n_s_fmt, __pyx_n_s_pixels, __pyx_n_s_rowlength); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_filename, __pyx_n_s_data, __pyx_n_s_kwargs, __pyx_n_s_w, __pyx_n_s_h, __pyx_n_s_fmt, __pyx_n_s_pixels, __pyx_n_s_rowlength); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_init, 265, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_init, 267, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 267, __pyx_L1_error)
 
-  /* "_curly.pyx":271
+  /* "_curly.pyx":273
  *         super(ImageLoaderMemory, self).__init__(filename, **kwargs)
  * 
  *     def load(self, kwargs):             # <<<<<<<<<<<<<<
  *         return self._data
  * 
  */
-  __pyx_tuple__22 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_load, 271, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_load, 273, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 273, __pyx_L1_error)
 
-  /* "_curly.pyx":464
+  /* "_curly.pyx":466
  * 
  * 
  * def request(url, callback, headers=None,             # <<<<<<<<<<<<<<
  *             method="GET", params=None, data=None, json=None,
  *             auth=None, cache_fn=None, preload_image=False,
  */
-  __pyx_tuple__24 = PyTuple_Pack(22, __pyx_n_s_url, __pyx_n_s_callback, __pyx_n_s_headers, __pyx_n_s_method, __pyx_n_s_params, __pyx_n_s_data, __pyx_n_s_json, __pyx_n_s_auth, __pyx_n_s_cache_fn, __pyx_n_s_preload_image, __pyx_n_s_priority, __pyx_n_s_no_image_cache, __pyx_n_s_qdata, __pyx_n_s_b_string, __pyx_n_s_c_header, __pyx_n_s_url_suffix, __pyx_n_s_key, __pyx_n_s_value, __pyx_n_s_postdata, __pyx_n_s_cache_dir, __pyx_n_s_header, __pyx_n_s_obj); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(22, __pyx_n_s_url, __pyx_n_s_callback, __pyx_n_s_headers, __pyx_n_s_method, __pyx_n_s_params, __pyx_n_s_data, __pyx_n_s_json, __pyx_n_s_auth, __pyx_n_s_cache_fn, __pyx_n_s_preload_image, __pyx_n_s_priority, __pyx_n_s_no_image_cache, __pyx_n_s_qdata, __pyx_n_s_b_string, __pyx_n_s_c_header, __pyx_n_s_url_suffix, __pyx_n_s_key, __pyx_n_s_value, __pyx_n_s_postdata, __pyx_n_s_cache_dir, __pyx_n_s_header, __pyx_n_s_obj); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 466, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(12, 0, 22, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_request, 464, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(12, 0, 22, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_request, 466, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 466, __pyx_L1_error)
 
-  /* "_curly.pyx":609
+  /* "_curly.pyx":611
  * 
  * 
  * def download_image(*args, **kwargs):             # <<<<<<<<<<<<<<
  *     """A wrapper around :func:`request` that set `preload_image` to True
  *     """
  */
-  __pyx_tuple__26 = PyTuple_Pack(2, __pyx_n_s_args, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 609, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(2, __pyx_n_s_args, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 611, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_download_image, 609, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 609, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_download_image, 611, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 611, __pyx_L1_error)
 
-  /* "_curly.pyx":616
+  /* "_curly.pyx":618
  * 
  * 
  * def process(*args):             # <<<<<<<<<<<<<<
  *     """Process results. It must be called as must as possible in order
  *     to process the results from the download threads.
  */
-  __pyx_tuple__28 = PyTuple_Pack(6, __pyx_n_s_args, __pyx_n_s_result, __pyx_n_s_data, __pyx_n_s_b_data, __pyx_n_s_callback, __pyx_n_s_item); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 616, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(6, __pyx_n_s_args, __pyx_n_s_result, __pyx_n_s_data, __pyx_n_s_b_data, __pyx_n_s_callback, __pyx_n_s_item); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_process, 616, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 616, __pyx_L1_error)
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_process, 618, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 618, __pyx_L1_error)
 
-  /* "_curly.pyx":644
+  /* "_curly.pyx":646
  * 
  * 
  * def install():             # <<<<<<<<<<<<<<
  *     """Install a scheduler in the Kivy clock to call :func:`process`
  *     """
  */
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_install, 644, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 644, __pyx_L1_error)
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_install, 646, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 646, __pyx_L1_error)
 
-  /* "_curly.pyx":651
+  /* "_curly.pyx":653
  * 
  * 
  * def uninstall():             # <<<<<<<<<<<<<<
  *     """Uninstall the scheduler that call :func:`process` from the Kivy clock
  *     """
  */
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_uninstall, 651, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 651, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_uninstall, 653, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 653, __pyx_L1_error)
 
-  /* "_curly.pyx":657
+  /* "_curly.pyx":659
  * 
  * 
  * def stop():             # <<<<<<<<<<<<<<
  *     """Stop any threads working in the background.
  *     Any ongoing results or request will be stopped.
  */
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_stop, 657, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 657, __pyx_L1_error)
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_stop, 659, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 659, __pyx_L1_error)
 
-  /* "_curly.pyx":667
+  /* "_curly.pyx":669
  * 
  * 
- * def configure(num_threads=4, req_verify_peer=0):             # <<<<<<<<<<<<<<
+ * def configure(num_threads=4, req_verify_peer=0, useragent=None):             # <<<<<<<<<<<<<<
  *     """Configure the library before any invocation
  *     Any call after the using `request`, `download_image` or `get_info`
  */
-  __pyx_tuple__33 = PyTuple_Pack(2, __pyx_n_s_num_threads, __pyx_n_s_req_verify_peer); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 667, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(5, __pyx_n_s_num_threads, __pyx_n_s_req_verify_peer, __pyx_n_s_useragent, __pyx_n_s_b_string, __pyx_n_s_config_useragent); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 669, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_configure, 667, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 667, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_curly__curly_pyx, __pyx_n_s_configure, 669, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 669, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -11265,23 +11499,23 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_6_curly_CurlyResult) < 0) __PYX_ERR(0, 291, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6_curly_CurlyResult) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6_curly_CurlyResult.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6_curly_CurlyResult.tp_dictoffset && __pyx_type_6_curly_CurlyResult.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6_curly_CurlyResult.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CurlyResult, (PyObject *)&__pyx_type_6_curly_CurlyResult) < 0) __PYX_ERR(0, 291, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6_curly_CurlyResult) < 0) __PYX_ERR(0, 291, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CurlyResult, (PyObject *)&__pyx_type_6_curly_CurlyResult) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6_curly_CurlyResult) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
   __pyx_ptype_6_curly_CurlyResult = &__pyx_type_6_curly_CurlyResult;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -11478,19 +11712,17 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("_curly", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -11924,221 +12156,230 @@
  */
   __pyx_v_6_curly_config_num_threads = 4;
 
   /* "_curly.pyx":43
  * cdef int config_num_threads = 4
  * # very bad, will activate by default once we can check cacert.pem on android
  * cdef int config_req_verify_peer = 0             # <<<<<<<<<<<<<<
- * 
+ * cdef char *config_useragent = NULL
  * 
  */
   __pyx_v_6_curly_config_req_verify_peer = 0;
 
-  /* "_curly.pyx":191
+  /* "_curly.pyx":44
+ * # very bad, will activate by default once we can check cacert.pem on android
+ * cdef int config_req_verify_peer = 0
+ * cdef char *config_useragent = NULL             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_v_6_curly_config_useragent = NULL;
+
+  /* "_curly.pyx":193
  * 
  * 
  * def get_info():             # <<<<<<<<<<<<<<
  *     cdef curl_version_info_data *info
  *     dl_ensure_init()
  */
-  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_1get_info, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_1get_info, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_info, __pyx_t_6) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_info, __pyx_t_6) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "_curly.pyx":263
+  /* "_curly.pyx":265
  * 
  * 
  * class ImageLoaderMemory(ImageLoaderBase):             # <<<<<<<<<<<<<<
  *     # Internal loader for data loaded from SDL2
  *     def __init__(self, filename, data, **kwargs):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_ImageLoaderBase); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_ImageLoaderBase); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_Py3MetaclassPrepare(__pyx_t_6, __pyx_t_4, __pyx_n_s_ImageLoaderMemory, __pyx_n_s_ImageLoaderMemory, (PyObject *) NULL, __pyx_n_s_curly, (PyObject *) NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3MetaclassPrepare(__pyx_t_6, __pyx_t_4, __pyx_n_s_ImageLoaderMemory, __pyx_n_s_ImageLoaderMemory, (PyObject *) NULL, __pyx_n_s_curly, (PyObject *) NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
 
-  /* "_curly.pyx":265
+  /* "_curly.pyx":267
  * class ImageLoaderMemory(ImageLoaderBase):
  *     # Internal loader for data loaded from SDL2
  *     def __init__(self, filename, data, **kwargs):             # <<<<<<<<<<<<<<
  *         w, h, fmt, pixels, rowlength = data
  *         self._data = [ImageData(
  */
-  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_6_curly_17ImageLoaderMemory_1__init__, 0, __pyx_n_s_ImageLoaderMemory___init, NULL, __pyx_n_s_curly, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_6_curly_17ImageLoaderMemory_1__init__, 0, __pyx_n_s_ImageLoaderMemory___init, NULL, __pyx_n_s_curly, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  if (__Pyx_SetNameInClass(__pyx_t_7, __pyx_n_s_init, __pyx_t_9) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_7, __pyx_n_s_init, __pyx_t_9) < 0) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "_curly.pyx":271
+  /* "_curly.pyx":273
  *         super(ImageLoaderMemory, self).__init__(filename, **kwargs)
  * 
  *     def load(self, kwargs):             # <<<<<<<<<<<<<<
  *         return self._data
  * 
  */
-  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_6_curly_17ImageLoaderMemory_3load, 0, __pyx_n_s_ImageLoaderMemory_load, NULL, __pyx_n_s_curly, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_6_curly_17ImageLoaderMemory_3load, 0, __pyx_n_s_ImageLoaderMemory_load, NULL, __pyx_n_s_curly, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  if (__Pyx_SetNameInClass(__pyx_t_7, __pyx_n_s_load, __pyx_t_9) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_7, __pyx_n_s_load, __pyx_t_9) < 0) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "_curly.pyx":263
+  /* "_curly.pyx":265
  * 
  * 
  * class ImageLoaderMemory(ImageLoaderBase):             # <<<<<<<<<<<<<<
  *     # Internal loader for data loaded from SDL2
  *     def __init__(self, filename, data, **kwargs):
  */
-  __pyx_t_9 = __Pyx_Py3ClassCreate(__pyx_t_6, __pyx_n_s_ImageLoaderMemory, __pyx_t_4, __pyx_t_7, NULL, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_Py3ClassCreate(__pyx_t_6, __pyx_n_s_ImageLoaderMemory, __pyx_t_4, __pyx_t_7, NULL, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ImageLoaderMemory, __pyx_t_9) < 0) __PYX_ERR(0, 263, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ImageLoaderMemory, __pyx_t_9) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "_curly.pyx":278
+  /* "_curly.pyx":280
  * #
  * 
  * class CurlyError(Exception):             # <<<<<<<<<<<<<<
  *     """Exception raised when something was wrong during the request, when
  *     checking the result with `raise_for_status`.
  */
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 278, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_6 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 278, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_Py3MetaclassPrepare(__pyx_t_6, __pyx_t_4, __pyx_n_s_CurlyError, __pyx_n_s_CurlyError, (PyObject *) NULL, __pyx_n_s_curly, __pyx_kp_s_Exception_raised_when_something); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 278, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3MetaclassPrepare(__pyx_t_6, __pyx_t_4, __pyx_n_s_CurlyError, __pyx_n_s_CurlyError, (PyObject *) NULL, __pyx_n_s_curly, __pyx_kp_s_Exception_raised_when_something); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_9 = __Pyx_Py3ClassCreate(__pyx_t_6, __pyx_n_s_CurlyError, __pyx_t_4, __pyx_t_7, NULL, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 278, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_Py3ClassCreate(__pyx_t_6, __pyx_n_s_CurlyError, __pyx_t_4, __pyx_t_7, NULL, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_CurlyError, __pyx_t_9) < 0) __PYX_ERR(0, 278, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_CurlyError, __pyx_t_9) < 0) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "_curly.pyx":285
+  /* "_curly.pyx":287
  * 
  * 
  * class CurlyHTTPError(CurlyError):             # <<<<<<<<<<<<<<
  *     """If the request was ok, this exception is raised if the HTTP status
  *     code was indicating an issue with the HTTP requests.
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_CurlyError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_CurlyError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_6, __pyx_n_s_CurlyHTTPError, __pyx_n_s_CurlyHTTPError, (PyObject *) NULL, __pyx_n_s_curly, __pyx_kp_s_If_the_request_was_ok_this_excep); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_6, __pyx_n_s_CurlyHTTPError, __pyx_n_s_CurlyHTTPError, (PyObject *) NULL, __pyx_n_s_curly, __pyx_kp_s_If_the_request_was_ok_this_excep); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_9 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_CurlyHTTPError, __pyx_t_6, __pyx_t_7, NULL, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_CurlyHTTPError, __pyx_t_6, __pyx_t_7, NULL, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_CurlyHTTPError, __pyx_t_9) < 0) __PYX_ERR(0, 285, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_CurlyHTTPError, __pyx_t_9) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "_curly.pyx":464
+  /* "_curly.pyx":466
  * 
  * 
  * def request(url, callback, headers=None,             # <<<<<<<<<<<<<<
  *             method="GET", params=None, data=None, json=None,
  *             auth=None, cache_fn=None, preload_image=False,
  */
-  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_3request, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_3request, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 466, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_request, __pyx_t_6) < 0) __PYX_ERR(0, 464, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_request, __pyx_t_6) < 0) __PYX_ERR(0, 466, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "_curly.pyx":609
+  /* "_curly.pyx":611
  * 
  * 
  * def download_image(*args, **kwargs):             # <<<<<<<<<<<<<<
  *     """A wrapper around :func:`request` that set `preload_image` to True
  *     """
  */
-  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_5download_image, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 609, __pyx_L1_error)
+  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_5download_image, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 611, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_download_image, __pyx_t_6) < 0) __PYX_ERR(0, 609, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_download_image, __pyx_t_6) < 0) __PYX_ERR(0, 611, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "_curly.pyx":616
+  /* "_curly.pyx":618
  * 
  * 
  * def process(*args):             # <<<<<<<<<<<<<<
  *     """Process results. It must be called as must as possible in order
  *     to process the results from the download threads.
  */
-  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_7process, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 616, __pyx_L1_error)
+  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_7process, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_process, __pyx_t_6) < 0) __PYX_ERR(0, 616, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_process, __pyx_t_6) < 0) __PYX_ERR(0, 618, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "_curly.pyx":644
+  /* "_curly.pyx":646
  * 
  * 
  * def install():             # <<<<<<<<<<<<<<
  *     """Install a scheduler in the Kivy clock to call :func:`process`
  *     """
  */
-  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_9install, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 644, __pyx_L1_error)
+  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_9install, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 646, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_install, __pyx_t_6) < 0) __PYX_ERR(0, 644, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_install, __pyx_t_6) < 0) __PYX_ERR(0, 646, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "_curly.pyx":651
+  /* "_curly.pyx":653
  * 
  * 
  * def uninstall():             # <<<<<<<<<<<<<<
  *     """Uninstall the scheduler that call :func:`process` from the Kivy clock
  *     """
  */
-  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_11uninstall, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 651, __pyx_L1_error)
+  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_11uninstall, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 653, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_uninstall, __pyx_t_6) < 0) __PYX_ERR(0, 651, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_uninstall, __pyx_t_6) < 0) __PYX_ERR(0, 653, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "_curly.pyx":657
+  /* "_curly.pyx":659
  * 
  * 
  * def stop():             # <<<<<<<<<<<<<<
  *     """Stop any threads working in the background.
  *     Any ongoing results or request will be stopped.
  */
-  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_13stop, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 657, __pyx_L1_error)
+  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_13stop, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 659, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_stop, __pyx_t_6) < 0) __PYX_ERR(0, 657, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_stop, __pyx_t_6) < 0) __PYX_ERR(0, 659, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "_curly.pyx":667
+  /* "_curly.pyx":669
  * 
  * 
- * def configure(num_threads=4, req_verify_peer=0):             # <<<<<<<<<<<<<<
+ * def configure(num_threads=4, req_verify_peer=0, useragent=None):             # <<<<<<<<<<<<<<
  *     """Configure the library before any invocation
  *     Any call after the using `request`, `download_image` or `get_info`
  */
-  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_15configure, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 667, __pyx_L1_error)
+  __pyx_t_6 = PyCFunction_NewEx(&__pyx_mdef_6_curly_15configure, NULL, __pyx_n_s_curly); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 669, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_configure, __pyx_t_6) < 0) __PYX_ERR(0, 667, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_configure, __pyx_t_6) < 0) __PYX_ERR(0, 669, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "_curly.pyx":1
  * # -*- coding: utf-8 -*-             # <<<<<<<<<<<<<<
  * 
  * # Cython import
  */
@@ -12270,15 +12511,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -12855,15 +13096,15 @@
     return __Pyx_GetBuiltinName(name);
 }
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = func->ob_type->tp_call;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -13290,15 +13531,15 @@
         return __Pyx_PyFunction_FastCall(func, &arg, 1);
     }
 #endif
     if (likely(PyCFunction_Check(func))) {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
             return __Pyx_PyObject_CallMethO(func, arg);
 #if CYTHON_FAST_PYCCALL
-        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
+        } else if (__Pyx_PyFastCFunction_Check(func)) {
             return __Pyx_PyCFunction_FastCall(func, &arg, 1);
 #endif
         }
     }
     return __Pyx__PyObject_CallOneArg(func, arg);
 }
 #else
@@ -14117,25 +14358,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -14172,14 +14431,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -14692,15 +14953,16 @@
     {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), PY_WRITE_RESTRICTED, 0},
     {0, 0, 0,  0, 0}
 };
 static PyObject *
 __Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, CYTHON_UNUSED PyObject *args)
 {
 #if PY_MAJOR_VERSION >= 3
-    return PyUnicode_FromString(m->func.m_ml->ml_name);
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
 #else
     return PyString_FromString(m->func.m_ml->ml_name);
 #endif
 }
 static PyMethodDef __pyx_CyFunction_methods[] = {
     {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
     {0, 0, 0, 0}
@@ -14895,14 +15157,17 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -14963,20 +15228,23 @@
     0,
     0,
     0,
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+    0,
+#endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
     }
     return 0;
@@ -15115,15 +15383,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -15209,41 +15477,48 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -15254,34 +15529,49 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -15396,45 +15686,14 @@
 bad:
     if (kwargs != __pyx_print_kwargs)
         Py_XDECREF(kwargs);
     return -1;
 }
 #endif
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
@@ -15449,45 +15708,14 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-    }
-}
-
 /* PrintOne */
 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION < 3
 static int __Pyx_PrintOne(PyObject* f, PyObject *o) {
     if (!f) {
         if (!(f = __Pyx_GetStdout()))
             return -1;
     }
@@ -15517,17 +15745,62 @@
         return -1;
     res = __Pyx_Print(stream, arg_tuple, 1);
     Py_DECREF(arg_tuple);
     return res;
 }
 #endif
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -15706,17 +15979,62 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -15997,19 +16315,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -16259,14 +16599,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `pycurly-1.0.1/curly/_curly.pyx` & `pycurly-1.0.3/curly/_curly.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 cdef SDL_sem *dl_sem
 cdef SDL_atomic_t dl_done
 cdef SDL_atomic_t dl_ready_to_process
 
 cdef int config_num_threads = 4
 # very bad, will activate by default once we can check cacert.pem on android
 cdef int config_req_verify_peer = 0
+cdef char *config_useragent = NULL
 
 
 cdef size_t _curl_write_data(void *ptr, size_t size, size_t nmemb, dl_queue_data *data) nogil:
     cdef:
         size_t index = data.size
         size_t n = (size * nmemb)
         char* tmp
@@ -81,15 +82,14 @@
     cdef:
         dl_queue_data *data
         CURL *curl
         SDL_RWops *rw
         int require_download
         FILE *fp
 
-
     curl = curl_easy_init()
     if not curl:
         return -1
 
     while SDL_AtomicGet(&dl_done) == 0:
         SDL_SemWait(dl_sem)
         data = <dl_queue_data *>queue_pop_first(&ctx_download)
@@ -110,14 +110,16 @@
             curl_easy_setopt(curl, CURLOPT_HEADERDATA, data)
             curl_easy_setopt(curl, CURLOPT_FOLLOWLOCATION, <void *><long>1L)
             # curl_easy_setopt(curl, CURLOPT_VERBOSE, <void *><long>1L)
             if data.headers != NULL:
                 curl_easy_setopt(curl, CURLOPT_HTTPHEADER, data.headers)
             else:
                 curl_easy_setopt(curl, CURLOPT_HTTPHEADER, NULL)
+            if config_useragent != NULL:
+                curl_easy_setopt(curl, CURLOPT_USERAGENT, config_useragent)
             if data.auth_userpwd != NULL:
                 curl_easy_setopt(curl, CURLOPT_HTTPAUTH, CURLAUTH_ANY)
                 curl_easy_setopt(curl, CURLOPT_USERPWD, data.auth_userpwd)
             if data.postdata != NULL:
                 curl_easy_setopt(curl, CURLOPT_POSTFIELDS, data.postdata)
                 curl_easy_setopt(curl, CURLOPT_POSTFIELDSIZE, strlen(data.postdata))
             if strncmp(data.method, "GET", 3) == 0:
@@ -660,15 +662,15 @@
     """
     uninstall()
     SDL_AtomicSet(&dl_done, 1)
     SDL_SemPost(dl_sem)
     SDL_DestroySemaphore(dl_sem)
 
 
-def configure(num_threads=4, req_verify_peer=0):
+def configure(num_threads=4, req_verify_peer=0, useragent=None):
     """Configure the library before any invocation
     Any call after the using `request`, `download_image` or `get_info`
     won't use the information and raise an exception.
 
     :Parameters:
         `num_threads`: int
             Number of background threads to use for downloading
@@ -680,7 +682,13 @@
             Defaults to False
     """
     if dl_running:
         raise Exception("Library already running, cannot reconfigure.")
     global config_num_threads, config_req_verify_peer
     config_num_threads = num_threads
     config_req_verify_peer = 1 if req_verify_peer else 0
+
+    cdef bytes b_string
+    if useragent:
+        b_string = useragent.encode("utf8")
+        config_useragent = strdup(b_string)
+
```

### Comparing `pycurly-1.0.1/curly/_include.pxi` & `pycurly-1.0.3/curly/_include.pxi`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         CURLOPT_HTTPPOST
         CURLOPT_HTTPGET
         CURLOPT_POSTFIELDS
         CURLOPT_HTTPAUTH
         CURLOPT_USERPWD
         CURLOPT_POSTFIELDSIZE
         CURLOPT_SSL_VERIFYPEER
+        CURLOPT_USERAGENT
         CURLAUTH_ANY
 
     enum CURLversion:
         CURLVERSION_NOW
 
     enum CURLSHcode:
         CURLSHE_OK
```

### Comparing `pycurly-1.0.1/curly/_queue.pxi` & `pycurly-1.0.3/curly/_queue.pxi`

 * *Files identical despite different names*

### Comparing `pycurly-1.0.1/pycurly.egg-info/PKG-INFO` & `pycurly-1.0.3/pycurly.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pycurly
-Version: 1.0.1
-Summary: UNKNOWN
-Home-page: UNKNOWN
-Author: UNKNOWN
-Author-email: UNKNOWN
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
+Version: 1.0.3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pycurly-1.0.1/setup.py` & `pycurly-1.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,61 @@
-# -*- coding: utf-8 -*-
-
 import sys
 from os import environ, getenv
 from os.path import join, isdir
 try:
     from setuptools import setup, Extension
 except ImportError:
     from distutils.core import setup, Extension
 
+
 def pkgconfig(*packages, **kw):
     flag_map = {'-I': 'include_dirs', '-L': 'library_dirs', '-l': 'libraries'}
+    for name in flag_map.values():
+        kw.setdefault(name, [])
     lenviron = None
     pconfig = join(sys.prefix, 'libs', 'pkgconfig')
 
     if isdir(pconfig):
         lenviron = environ.copy()
         lenviron['PKG_CONFIG_PATH'] = '{};{}'.format(
             environ.get('PKG_CONFIG_PATH', ''), pconfig)
     cmd = 'pkg-config --libs --cflags {}'.format(' '.join(packages))
     results = getoutput(cmd, lenviron).split()
     for token in results:
         ext = token[:2].decode('utf-8')
         flag = flag_map.get(ext)
         if not flag:
             continue
-        kw.setdefault(flag, []).append(token[2:].decode('utf-8'))
+        kw[flag].append(token[2:].decode('utf-8'))
     return kw
 
 
 def getoutput(cmd, env=None):
     import subprocess
-    p = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE,
-                         stderr=subprocess.PIPE, env=env)
+    p = subprocess.Popen(cmd,
+                         shell=True,
+                         stdout=subprocess.PIPE,
+                         stderr=subprocess.PIPE,
+                         env=env)
     p.wait()
     if p.returncode:  # if not returncode == 0
-        print('WARNING: A problem occurred while running {0} (code {1})\n'
-              .format(cmd, p.returncode))
+        print('WARNING: A problem occurred while running {0} (code {1})\n'.
+              format(cmd, p.returncode))
         stderr_content = p.stderr.read()
         if stderr_content:
             print('{0}\n'.format(stderr_content))
         return ""
     return p.stdout.read()
 
 
 # version
 with open(join("curly", "__init__.py")) as fd:
     versionline = [x for x in fd.readlines() if x.startswith("__version__")]
     VERSION = versionline[0].split('"')[-2]
 
-
 FILES = [
     'curly/_curly.pyx',
     'curly/_include.pxi',
     'curly/_queue.pxi',
 ]
 
 LIBRARIES = []
@@ -65,31 +68,28 @@
     "name": "pycurly",
     "version": VERSION,
     "packages": ["curly"],
     "py_modules": ["setup"],
     "ext_package": "curly",
     "package_data": {},
     "classifiers": [
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Developers",
+        "Development Status :: 4 - Beta", "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
-        "Natural Language :: English",
-        "Operating System :: MacOS",
+        "Natural Language :: English", "Operating System :: MacOS",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Topic :: Software Development :: Libraries :: Application Frameworks"
     ]
 }
 
-
 # check platform
 platform = sys.platform
 ndkplatform = environ.get('NDKPLATFORM')
 if ndkplatform is not None and environ.get('LIBLINK'):
     platform = 'android'
 kivy_ios_root = environ.get('KIVYIOSROOT', None)
 if kivy_ios_root is not None:
@@ -114,55 +114,54 @@
 cython_directives = {}
 define_macros = []
 if with_coverage:
     cython_directives["binding"] = True
     cython_directives["embedsignature"] = True
     cython_directives["profile"] = True
     cython_directives["linetrace"] = True
-    define_macros = [
-        ("CYTHON_PROFILE", 1),
-        ("CYTHON_TRACE", 1),
-        ("CYTHON_TRACE_NOGIL", 1)]
+    define_macros = [("CYTHON_PROFILE", 1), ("CYTHON_TRACE", 1),
+                     ("CYTHON_TRACE_NOGIL", 1)]
 
 # find libraries
 if platform == "android":
     # XXX untested yet
     INCLUDE_DIRS = getenv("INCLUDE_DIRS").split(":")
     LIBRARIES = ["SDL2", "curl", "SDL2_image"]
     LIBRARY_DIRS = ["libs/" + getenv("ARCH")]
 elif platform == "ios":
     sysroot = environ.get("IOSSDKROOT", environ.get("SDKROOT"))
     if not sysroot:
         raise Exception("IOSSDKROOT is not set")
     INCLUDE_DIRS = [sysroot]
     LIBRARIES = []
     LIBRARY_DIRS = []
+elif platform == "win32":
+    INCLUDE_DIRS.append(join(getenv("CONDA_PREFIX"), "Lib", "include"))
+    LIBRARY_DIRS.append(join(getenv("CONDA_PREFIX"), "Lib", "lib"))
+    LIBRARIES = ["SDL2", "curl", "SDL2_image"]
 else:
     flags = pkgconfig("sdl2", "SDL2_image", "libcurl")
     INCLUDE_DIRS.extend(flags["include_dirs"])
     LIBRARIES.extend(flags["libraries"])
+    LIBRARY_DIRS.extend(flags["library_dirs"])
 
 # create the extensions
 extensions = [
-    Extension(
-        "_curly", FILES,
-        libraries=LIBRARIES,
-        library_dirs=LIBRARY_DIRS,
-        include_dirs=INCLUDE_DIRS,
-        extra_link_args=EXTRA_LINK_ARGS,
-        define_macros=define_macros
-    )
+    Extension("_curly",
+              FILES,
+              libraries=LIBRARIES,
+              library_dirs=LIBRARY_DIRS,
+              include_dirs=INCLUDE_DIRS,
+              extra_link_args=EXTRA_LINK_ARGS,
+              define_macros=define_macros)
 ]
 if with_cython:
     from Cython.Build import cythonize
-    extensions = cythonize(
-        extensions, compiler_directives=cython_directives)
+    extensions = cythonize(extensions, compiler_directives=cython_directives)
 
 cmdclass = {'build_ext': build_ext}
 
 # create the extension
-setup(
-    cmdclass=cmdclass,
-    install_requires=INSTALL_REQUIRES,
-    ext_modules=extensions,
-    **SETUP_KWARGS
-)
+setup(cmdclass=cmdclass,
+      install_requires=INSTALL_REQUIRES,
+      ext_modules=extensions,
+      **SETUP_KWARGS)
```

